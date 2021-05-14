---
---

# README

## Domain Model Representation

There are a few ways to build a Personal Kanban with Jekyll so let me take a minute to outline domain model I am currently using. I represent **Stories** as Jekyll _posts_, **Milestones** and **Sprints** as Jekyll _categories_ and **Use Cases** as Jekyll _pages_. These mappings are certain to change once I get a bit deeper but I will update this README when that happens.

## Definitions

A **Use Case** formally describes a scenario which typical users will almost certainly find themselves in. I like to start planning with these. For me, they provide an overall view of the proposed software. A suite of Use Cases can generally describe an application. Use Cases are written from the user perspective and generally describe required functionality. Whenever possible, Use Cases should refrain from specifying the technicality of proposed solutions.

Use Cases map to **Stories** wich are typically considered a _unit of work_. In my case, I typically let Use Cases _drive_ the creation of Stories. A multi-step Use Case can easily contain several smaller, detailed development Stories to hone in on the details. Again, Stories should largely refrain from specifying technical solutions and should instead focus on features or functionality.

**Milestones** then refer to a subset of Stories, and indirectly then, a subset of whole or partial Use Cases. **Sprints** are simply a subset of the Stories associated with a Milestone.

## Overview

- Per Jekyll rules then, Stories masquerade as _blog posts_ in the appropriate \_posts directory.
- Stories should be kept in a ```sprint-XX``` or ```kanban/column``` directory.
- As part of the kanban board, there is only one set of kanban columns and so stories should physically move through said columns.

## Usage

- In general, users create Stories and store them in the relevant ```milestones/milestone-XX/sprint-XX/_posts``` directory for which they predict they will be worked. It is certainly reasonable to limit the number of such forecast directories and simply identify a ```backlog``` directory for anything not yet scheduled.
- Once a sprint becomes the active sprint, stories should be moved from the sprint directory wherein which they were forecast and moved to the appropriate ```kanban/column/_posts``` directory.
- Feel free to adjust as necessary for your needs. Part of the beauty of this system is that once you understand it, you should tailor the directories to your style.
- And of course, commit often. That is a major part of why this works so well for me.

## Future

- There are other ways to organize this board. We aren't using ```tags``` for instance.
- I have a few other views in mind.
- Explore the YAML to include things like acceptance criteria, begin and end timestamps etc.
- Reporting shouldn't be difficult since Jekyll would have no problem generating JSON files from YAML fields if we provided them.