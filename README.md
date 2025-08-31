# Employee Handbook
A guide that explains a company’s policies, rules, and workplace practices to help employees understand their rights, responsibilities, and work culture.

## Table of Contents
- [Employee Handbook](#employee-handbook)
  - [Table of Contents](#table-of-contents)
- [Roles \& Jobs](#roles--jobs)
  - [Roles](#roles)
  - [Jobs](#jobs)
- [Development process](#development-process)
  - [Overview](#overview)
  - [Product backlog](#product-backlog)
  - [Backlog Refinement](#backlog-refinement)
  - [Development \& Testing](#development--testing)
  - [Demo \& Feedback](#demo--feedback)
- [⌛Pending documents](#pending-documents)

# Roles & Jobs

> NOTE  
> In each project, roles may change depending on what best fits the project’s needs.

## Roles

The responsibilities or "hats" you take on within a team or project, which may shift depending on the situation.

```mermaid
graph LR
  PO["PO<br/>Product Owner"]
  PM["PM<br/>Project Manager"]
  PL["PL<br/>Project Leader"]
  TM["TM<br/>Team Member"]
  TL["TL<br/>Team Leader"]
  
  PO --> PM --> PL --> TL --> TM
```

| Role | Description |
|------|-------------|
| Product Owner | Defines the product vision and prioritizes the backlog. |
| Project Manager | Manages timelines, resources, and cross-team communication. |
| Project Leader | Understands project goals, ensures project plans are delivered, provides solutions and guidance to the team, aligns their efforts, and oversees planning and progress tracking. |
| Team Leader | Guides the team in best practices, addresses challenges, and regularly updates the *Project Leader*. |
| Team Member | Contributes to the project by completing assigned tasks and collaborating with others. |

## Jobs

The position you're hired for, responsible for specific tasks that contribute to completing the project the team is working on.

```mermaid
graph TB
  subgraph Dev["Developer teams"]
    direction TB
    FE[Front-end Team]
    BE[Back-end Team]
    M[Mobile Team]
  end
  subgraph RP["Resource pools"]
    direction TB
    D[Designer Team]
    DO[DevOps Team]
    QA[QA Team]
  end
```


| Team | Type | Description |
|------|------|-------------|
| Designer Team | Resource Pool | Creates the visual and interactive elements of the product. |
| DevOps Team | Resource Pool | Focuses on automating and optimizing the development and deployment processes. |
| QA Team | Resource Pool | Ensures the product meets quality standards through testing. |
| Front-end Team | Developer Team | Implements the user interface and ensures a seamless user experience. |
| Back-end Team | Developer Team | Works on server-side logic, databases, and APIs. |
| Mobile Team | Developer Team | Specializes in building applications for mobile devices.

# Development process

We follow **Agile** practices with incremental development and continuous feedback to guide our process.

![img](https://miro.medium.com/v2/resize:fit:828/1*FELa1FEHnPPTFuf5trq6ew.png)

## Overview

```mermaid
flowchart
  s0[**Requirement Gathering**<br/>Collect requirements and create user stories to add into the **Product Backlog**.]
  s1[[**Backlog Refinement**]]
  subgraph Sprint
    s2[**Choose Cards to Commit**<br/>Selects cards that can be delivered within the sprint.]
    s3[[**Development & Testing**]]
    s4[[**Demo & Feedback**]]
  end
  s5[Retrospective]

  s0 --> s1 --> Sprint
  s2 --> s3 --> s4 --> s5 --> s1
```

## Product backlog
It is the master prioritized to-do list for a product, representing everything that may be needed to improve, build, deploy, or maintain it.

## Backlog Refinement

It is the process of reviewing and improving backlog items by adding details & acceptance criteria, clarifying requirements, estimating effort, and re-prioritizing so they are ready for upcoming sprints.

```mermaid
stateDiagram-v2
  s1: **Backlog Refinement**<br/>Refine user stories by adding details, criteria, and estimates.
  s15: **Technical Exploration (Spike)**<br/>Run a time-boxed Spike to research and decide the best technical approaches.
  s2: **Prototyping**<br/>Convert user stories into prototypes and validate them with the Product Owner.
  s3: **Development Readiness**<br/>In this state, user stories are ready to be committed into the sprint.

  [*] --> s1
  s1 --> s2
  s1 --> s15: if technical uncertainty
  s15 --> s1
  s2 --> s3: if approved
  s3 --> [*]
```

## Development & Testing

Building features, writing tests, reviewing code, and validating functionality for delivery.

```mermaid
stateDiagram-v2
  s1: **Setup**<br/>The team selects a development ring, creates a new branch, and configures the build pipeline.
  s2: **Development**<br/>The team develops the feature in the chosen ring and writes unit tests.
  s3: **Testing**<br/>The team creates a Pull Request (PR) and tests the feature in the chosen ring when it is ready.
  s4: **Code Review**<br/>The Team Leader reviews the Pull Request and provides feedback.
  s5: **Demo Ready**<br/>The feature is prepared to be demonstrated to the **Product Owner** at the end of the sprint.

  [*] --> s1
  s1 --> s2
  s2 --> s3
  s3 --> s4
  s4 --> s5
  s5 --> [*]
  s3 --> s2: if tests fail
  s4 --> s2: if need to refactor
```

## Demo & Feedback

Show finished work to the **Product Owner** for review and feedback.

```mermaid
stateDiagram-v2
  s1: **Prepare Demo**<br/>The team ensures finished cards are ready to be demonstrated in the development environment.
  s2: **Run2 Demo**<br/>The team presents the completed features to the Product Owner.
  s3: **Collect Feedback**<br/>The Product Owner gives feedback or suggests improvements. These, along with deployment tasks to production, are recorded as new cards for the Product Owner to review and prioritize later.

  [*] --> s1
  s1 --> s2
  s2 --> s3
  s3 --> [*]
```

# ⌛Pending documents
1. Sprint planning
2. Team meetings
3. Cross-team collaboration
4. Daily routine
5. TBD