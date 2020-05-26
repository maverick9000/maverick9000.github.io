---
title: Upgrade to Grafana 7
layout: post
subtitle: and everything that will go wrong
description: and everything that will go wrong
image: /assets/img/uploads/grafana.jpg
date: '2020-05-26 13:28:05 +0900'
optimized_image: /assets/img/uploads/grafana.jpg
category: devops
tags:
  - monitoring
  - grafana
  - linux
author: Maverick Stoklosa
---

Grafana 7 is out and you want to upgrade. Reading through the Changelog it seems nothing could go wrong but it will.

First of all when you go to your alerts page you will get an error when you try to Test it

![grafana](/assets/img/uploads/grafana4.png)

You will have to edit the JSON of your model:

![grafana](/assets/img/uploads/grafana5.png)

Looking for the `notifications` sections like so

![grafana](/assets/img/uploads/grafana6.png)

and removing the { 'id': XX } parts. Only then will you be able to save and test your model.

If you are using variables inside your query you will see `no data`

For example something like this:

```
AND  ("account_id" =~ /^$account_id$/) AND  ("hostname" =~ /^$hostname$/) AND ("endpoint" =~/^$endpoint$/)
```

won't work in alert queries.

PhantomJS has been removed which means you won't be able to render images in your alert emails.

Instead you will see something like this

![grafana](/assets/img/uploads/grafana2.png)

But it's cool you anticipated that because the docs said you're gonna have to install the rendering plugin

`grafana-cli plugins install grafana-image-renderer`

Still no dice though. Only later will you realize Ubuntu requires some additional packages to make this work. 

```
apt install libx11-6 libx11-xcb1 libxcomposite1 libxcursor1 libxdamage1 libxext6 libxfixes3 libxi6 libxrender1 libxtst6 libglib2.0-0 libnss3 libcups2  libdbus-1-3 libxss1 libxrandr2 libgtk-3-0 libgtk-3-0 libasound2
```

and you're back in business

![grafana](/assets/img/uploads/grafana3.png)
