---
title: Agile Software Development Coles Notes
layout: post
date: '2020-04-20'
subtitle: TLDR
description: "Just give me the executive summary"
image: /assets/img/uploads/coles.jpg
optimized_image: /assets/img/uploads/coles.jpg
category: fundementals
tags:
  - fundementals
  - agile
  - scrum
  - kanban
  - scrumban
author: Maverick Stoklosa
---

'Lord of the Flies' I still have nightmares about passing the conch.

Here is what I learned about Agile from books like [Scrum: The Art of Doing Twice the Work in Half the Time](https://amzn.to/3eW64p1) and doing Agile Web Development for the past few years. It hasn't always been by the book but the general idea has always been there.

## Sprint

Once you decide what gets done in the sprint it's fixed in stone, it cannot be changed. The team must be autonomous in implementing the sprint.

## Roles

1. **Project sponsor:** the guy with the cash
1. **Business leaders:** people getting in the way asking for last minute changes and reprioritizing
1. **Senior user:** smart people using the app
1. **Business user:** people using the app
1. **Tech leader:** CTO

## Estimating

### BUS

#### Big
	- if you have many of these break them down into multiple small ones
	- Some will stay big because they cannot provide the necessary value to stake holders if they are altered

#### Uncertain
	- Requirements are vague

#### Small
	- you want most of the stories to be small effort ie. Can be done in a few days

### T Shirt Size

1. XS
1. S
1. M
1. L
1. XL

### Fibonacci Sequences
1. 1
1. 2
1. 3
1. 5
1. 8
1. 13
1. 21

## Versus Waterfall

![waterfall](/assets/img/uploads/agile_1.png)

A product increment is like a new version of an app with more features. In agile you take vertical slices versus a horizontal flow.

## Cons of Agile

- difficult to apply what you learned in one project to another because knowledge is siloed
- difficult to implement in a company using another methodology
- no one takes ownership of the project, all work together
* there isn't much documentation because you talk things through instead

## Agile is

* deliver value faster: don't have to wait for months before something they can use is deployed
* welcome change: as you work on the project  you learn things you didn't know in the beginning so don't throw out the new knowledge act on it and make the necessary changes
* deliver working software frequently: it should always be usable, every sprint needs to produce an MVP, this frequency is up to you, 1 week or 2 weeks
* work daily together the biz team and dev team are working in the same room on the same project - collaborative discussion with team and client
* put together a team of motivated individuals and give them the tools to get it done and trust them to do it - no need to manage them. Each player is a problem solver not a 'coder' or 'manager'. You have to do many jobs. Your responsibility goes beyond your title.
* continuous pace, not spurts of OT, not all the pressure on one part of the team
* software can be large and daunting project so focus on one part you can build out and expand from there
* client assumes that what they say at the beginning is the scope and cannot be changed so they tell you all their wishes even though most are not providing value. If you allow for change then they can come up with better requirements later on when they have an MVP and have used it for a while.
* Introspective, end of sprint: what went well, what can be improved

![lifecycle](/assets/img/uploads/agile_2.png)

## Kanban

- Came from Toyota
* Jira / Trello is Kanban

![kanban](/assets/img/uploads/agile_3.png)

- Don't want multiple WIP you want to start and finish tasks 
- In JIRA you can limit the amount of WIP tasks allowed, i.e. 1 per developer
JIRA warns you If something is blocking or if there's too many WIP

![kanban](/assets/img/uploads/agile_4.png)

- Grouped by department or priority etc
- Red = highest priority

### You can categorize as:

* Todo: not fully specced yet
* Ready: specced, can be moved to WIP
* In progress; WIP
* Done: Completed

## Scrumban 

### Pull/Push Issues
In Kanban you pull work - you take ownership
In scrum you're assigned the work
In Scrumban you pull the work

### Limits
Kanban WIP limits

### Roles
Scrum has clear roles
Kanban has no roles - everyone is on same team
Scrumban doesn’t have set roles but may have specialized roles

### Board
Kanban style
:
Kanban Todo -> Backlog

![scrumban](/assets/img/uploads/agile_5.png)

#### Triage/Feature Freeze towards end of project

What are the priority tickets and freeze the rest of the work: only high priority items are done in triage stage
