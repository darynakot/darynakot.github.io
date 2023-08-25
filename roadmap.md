---
layout: default
title: Roadmap
description: How to build the Technology Roadmap?
---
<script src="https://unpkg.com/mermaid@10.4.0/dist/mermaid.min.js"></script>

<div class="mermaid">
flowchart LR
    A[/Home/]:::foo ~~~ B[/SDLC\]:::foo
    B ~~~ C[\Roadmap\]:::foo
    C ~~~ D[\RACI Matrix/]:::foo
    D ~~~ E[/PM Tools/]:::foo
    E ~~~ H[/Conway's Law\]:::foo
    classDef foo fill:#155799, #159957,stroke:#fff,color:#fff
    click A "https://darynakot.github.io/" _blank
    click B "https://darynakot.github.io/sdlc.html" _blank
    click C "https://darynakot.github.io/roadmap.html" _blank
    click D "https://darynakot.github.io/raci.html" _blank
    click E "https://darynakot.github.io/pmtools.html" _blank
    click H "https://darynakot.github.io/conways-law.html" _blank
</div>

Within an Agile team, the Product Owner is often responsible for managing not only the product backlog but defining the project’s vision and priorities. One of the ways they define the project’s vision is with an Agile product roadmap. 

Agile roadmap is a long-term, high-level overview of the product’s expected evolution. It should not be confused with the backlog as the roadmap is not where individual project tasks are planned. It is rather where vision meets strategy.

## Benefits of an Agile roadmap
1. Providing a high-level overview for stakeholders
2. Giving teams insight into priorities and timelines as context for day-to-day tasks
3. Explaining the project’s importance — both for the organization and the user/customer
4. Articulating long-term strategy 

## Types of Agile roadmaps
In a project management setting that is hyperfocused on individual tasks, a product roadmap is the big picture planning needed in order to focus teams, get stakeholder buy-in, and anticipate growth. Two popular types of Agile roadmaps include progress-based and time-based roadmaps. 

### Time-based roadmap
As its name suggests, a time-based roadmap focuses on how the project will evolve over a certain period of time. This can be looked at in weeks, months, quarters, or even years. Stakeholders may find it especially valuable because it clarifies expected timelines and key releases without getting bogged down into day-to-day processes.

<div class="mermaid">
gantt
    title Time-based roadmap
    dateFormat  YYYY-MM-DD
    excludes    weekends
    section A section
    Completed task            :done,    des1, 2023-01-06,2023-01-08
    Active task               :active,  des2, 2023-01-09, 3d
    Future task               :         des3, after des2, 5d
    Future task2              :         des4, after des3, 5d

    section Critical tasks
    Completed task in the critical line :crit, done, 2023-01-06,24h
    Implement parser and jison          :crit, done, after des1, 2d
    Create tests for parser             :crit, active, 3d
    Future task in critical line        :crit, 5d
    Create tests for renderer           :2d
    Add to mermaid                      :1d
    Functionality added                 :milestone, 2023-01-25, 0d

    section Documentation
    Describe gantt syntax               :active, a1, after des1, 3d
    Add gantt diagram to demo page      :after a1  , 20h
    Add another diagram to demo page    :doc1, after a1  , 48h

    section Last section
    Describe gantt syntax               :after doc1, 3d
    Add gantt diagram to demo page      :20h
    Add another diagram to demo page    :48h
</div>

### Progress-based roadmap
A progress-based roadmap takes a “to-do” → “in progress” → “complete” approach to road mapping and is often represented through a Kanban-like board. It focuses more on making progress on critical features and releases, as opposed to meticulously following timelines or predetermined time frames.

A roadmap is an important piece of documentation, but it should not be treated as something set in stone. Because Agile’s values and principles emphasize adapting to change, the roadmap can, and should, evolve based on what is learned in each iterative cycle as the project progresses.

[Source](https://www.wrike.com/project-management-guide/faq/what-is-an-agile-roadmap/)
