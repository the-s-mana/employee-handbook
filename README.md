# Employee Handbook
A guide that explains a company’s policies, rules, and workplace practices to help employees understand their rights, responsibilities, and work culture.

# 1. Roles & Jobs

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

# 2. Development process

We follow **Agile** practices with incremental development and continuous feedback to guide our process.

![img](https://miro.medium.com/v2/resize:fit:828/1*FELa1FEHnPPTFuf5trq6ew.png)

## Overview

```mermaid
flowchart
  s0[**Requirement Gathering**<br/>Collect requirements and create user stories to add into the Product Backlog.]
  s1[[**Backlog Refinement**]]
  subgraph Sprint
    s2[**Choose Cards to Commit**<br/>Selects cards that can be delivered within the sprint.]
    s3[[**Development & Testing**]]
    s4[**Demo & Feedback**]
  end
  s5[Retrospective]

  s0 --> s1 --> Sprint
  s2 --> s3 --> s4 --> s5 --> s1
```

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
TBD

# Daily routine
TBD
