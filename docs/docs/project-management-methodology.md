---
sidebar_position: 3
sidebar_label: Project Management Methodology
---

# Project Management Methodology

Effective project management ensures that software development efforts are organised, efficient, and aligned with project goals. While many methodologies exist, it is important to select an approach that balances structure, collaboration, and adaptability.

To determine the best fit for our team and project, we researched and evaluated several project management methodologies and tools. Below we document the options considered, their strengths and weaknesses, and the rationale for our chosen approach.

### Waterfall

**Overview:**  
Waterfall is a linear, sequential approach where each phase of development (requirements, design, implementation, testing, deployment) is completed before the next begins. It is best suited for projects with clearly defined requirements and low uncertainty.

![Waterfall](/img/waterfall.png)

**Resources:**
- [Waterfall Model – TutorialsPoint](https://www.tutorialspoint.com/sdlc/sdlc_waterfall_model.htm)  
- [Atlassian Guide to Waterfall](https://www.atlassian.com/agile/project-management/waterfall-vs-agile)

**Strengths**
- Clear and predictable process with well-defined phases.  
- Easy to measure progress and milestones.  
- Works well for projects with fixed requirements and low uncertainty.

**Weaknesses**
- Inflexible to changes or evolving requirements.  
- Late discovery of issues, as testing occurs near the end of the cycle.  
- Limited stakeholder feedback during development.

### Kanban

**Overview:**  
Kanban is a visual workflow management method using a board and cards to track tasks. It focuses on continuous delivery and limiting work in progress, providing flexibility and visualisation of the workflow.


**Resources:**
- [Kanban Guide – Atlassian](https://www.atlassian.com/agile/kanban)  
- [Kanban Principles](https://www.kanbanize.com/kanban-resources/getting-started/what-is-kanban)

**Strengths**
- Flexible and lightweight.  
- Visualises workflow and identifies bottlenecks.  
- Supports continuous delivery without strict time-boxed iterations.

**Weaknesses**
- Lacks structure for prioritisation or planning at scale.  
- Can be less effective for teams needing strict deadlines.  
- Minimal formal guidance on roles and responsibilities.

### Agile

**Overview:**  
Agile is an **iterative and adaptive approach** to software development that emphasises collaboration, customer feedback, and rapid delivery of functional software. Agile prioritises working software over comprehensive documentation, responding to change over following a fixed plan, and close interaction between teams and stakeholders.

![Agile](/img/agile.jpg)

**Resources:**
- [Agile Manifesto](https://agilemanifesto.org/)  
- [Agile Methodology – Atlassian](https://www.atlassian.com/agile)

**Strengths**
- **Adaptable to change** – Responds quickly to evolving requirements.  
- **Collaboration-focused** – Encourages strong communication among developers, stakeholders, and users.  
- **Early and continuous value delivery** – Functional software delivered in short iterations with continuous improvement.

**Weaknesses**
- **Less predictable timelines** – Iterative cycles can make long-term delivery estimation challenging.  
- **Requires discipline** – Strong communication, consistent feedback, and adherence to Agile principles are necessary.  
- **Scaling challenges** – Can be harder to scale for larger or complex projects without defined frameworks.

### Scrum

**Overview:**  
Scrum is a **structured Agile framework** that organises work into time-boxed sprints (1–4 weeks) and defines roles such as Product Owner, Scrum Master, and Development Team. It provides ceremonies and artefacts for visibility, accountability, and predictability.

![Scrum](/img/scrum.png)

**Resources:**
- [Scrum Guide](https://www.scrumguides.org/)  
- [Scrum Overview – Scrum Alliance](https://www.scrumalliance.org/why-scrum)

**Strengths**
- **Clear roles and responsibilities** – Ensures accountability for planning, delivery, and quality.  
- **Frequent feedback** – Sprint reviews and retrospectives facilitate continuous improvement.  
- **Progress visibility** – Artefacts like product backlog, sprint backlog, and burndown charts provide transparency.

**Weaknesses**
- **Ceremony overhead** – Regular stand-ups, sprint planning, and retrospectives require commitment.  
- **Risk of rigidity** – Mechanical adherence can slow adaptability.  
- **Overhead for small teams** – May introduce unnecessary complexity for very small or highly flexible teams.

### GitHub Projects

**Overview:**  
GitHub Projects is a tool for task and workflow management integrated with the repository, often using Kanban-style boards. It is especially useful for teams already using GitHub for version control.

**Resources:**
- [GitHub Projects Guide](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects)

**Strengths**
- **Integrated Task Management** – Links tasks, issues, and code for transparency and centralisation.  
- Visibility of tasks, ownership, and progress.  
- Supports automation, e.g., moving cards when PRs are merged.  
- Lightweight and easy to adopt.

**Weaknesses**
- Less advanced than dedicated PM tools (e.g., Jira, Trello).  
- Limited reporting and analytics.  
- Requires consistent maintenance to avoid clutter.

## Options Considered

| Methodology / Tool | Structure | Flexibility | Collaboration | Ease of Use | Transparency |
|-------------------|-----------|------------|---------------|------------|-------------|
| Waterfall         | High      | Low        | Medium        | Medium     | High        |
| Kanban            | Medium    | High       | High          | High       | Medium      |
| Agile             | Medium    | High       | High          | Medium     | High        |
| Scrum             | High      | Medium     | High          | Medium     | High        |
| GitHub Projects   | Low       | High       | High          | High       | High        |

We evaluated each methodology and tool against **structure, flexibility, collaboration, ease of use, and transparency**. Waterfall was ruled out due to low adaptability, while Kanban alone lacked sufficient structure for sprint planning. Combining Agile, Scrum, and GitHub Projects provided the best balance of flexibility, structure, and visibility.

## Our Choice: Agile + Scrum + GitHub Projects

After evaluation, we selected **Agile as our overarching methodology**, **Scrum as our process framework**, and **GitHub Projects as our task management tool**.

**Reasons for this choice**
- **Iterative and Adaptive** – Responds quickly to changing requirements.  
- **Structured Collaboration** – Scrum provides roles, ceremonies, and sprint planning.  
- **Integrated and Centralised Task Management** – GitHub Projects links tasks, issues, and code.  
- **Team Visibility and Accountability** – Everyone can track progress, responsibilities, and dependencies.

**Conclusion:**  
Combining Agile, Scrum, and GitHub Projects allows us to **maintain structure while staying flexible**, ensuring development is organised, collaborative, and responsive to user needs.

**References:**
1. Agile Manifesto, [https://agilemanifesto.org](https://agilemanifesto.org)  
2. Atlassian Guides – Agile, Kanban, Waterfall, [https://www.atlassian.com/agile](https://www.atlassian.com/agile)  
3. Scrum Guide, [https://www.scrumguides.org](https://www.scrumguides.org)