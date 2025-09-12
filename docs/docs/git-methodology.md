---
sidebar_position: 5
sidebar_label: Git Methodology
---

# Git Methodology

Git, by design, is a **non-opinionated tool**. Linus Torvalds, its creator, even described Git as a “stupid content tracker,” emphasising that Git itself does not enforce any particular workflow or branching strategy. This flexibility is powerful, but it also places the responsibility on teams to define opinionated practices that bring structure and consistency. Without a clear workflow, collaboration can become fragmented, leading to issues such as conflicting changes, unstable releases, or inefficient integration cycles.

To ensure effective collaboration and maintain code quality, our team researched and evaluated several widely recognised **Git workflows**. Below we document the methodologies considered, their strengths and weaknesses, and the rationale for our chosen approach.

### Git Flow

**Overview:**  
Git Flow is a branching strategy ideal for projects with formal release cycles. It introduces multiple long-lived branches (e.g., `main`, `develop`, `release`, `hotfix`) and enforces strict rules for merging and releases. This methodology is particularly useful for projects with clearly defined versioning and staged environments.

![Git Flow](/img/git-flow.png)

**Resources:**
- [Original Git Flow by Vincent Driessen](https://nvie.com/posts/a-successful-git-branching-model/)  
- [Atlassian Git Flow Guide](https://www.atlassian.com/git/tutorials/comparing-workflows/git-flow)

**Strengths**
- Strong release management and branch separation.  
- Well-defined structure for complex projects.  
- Stable production environment due to branch discipline.  
- Supports multiple parallel versions in production.

**Weaknesses**
- Heavyweight and complex for new contributors.  
- Slower integration cycles due to reliance on multiple long-lived branches.  
- Merge conflicts and overhead from managing many branches.  
- Overly formal for teams prioritising agility or continuous delivery.

### GitHub Flow

**Overview:**  
GitHub Flow is a lightweight branching strategy designed for continuous deployment. Developers create short-lived feature branches, open pull requests (PRs), and merge back into `main` after code review and testing. It is simple, agile, and highly compatible with modern CI/CD practices.

![GitHub Flow](/img/github-flow.png)

**Resources:**
- [GitHub Flow Guide](https://docs.github.com/en/get-started/quickstart/github-flow)  
- [GitHub Flow Explained](https://guides.github.com/introduction/flow/)

**Strengths**
- Simple and easy to adopt, even for small teams.  
- Encourages collaboration and transparency via PRs.  
- Ideal for continuous integration and deployment.  
- Promotes short-lived branches, reducing merge conflicts.  
- Supports rapid feature delivery and iterative development.

**Weaknesses**
- Minimal release structure; less suited for complex versioning.  
- Can be challenging for larger teams without strong discipline.  
- Requires robust testing and CI/CD to maintain stability of `main`.  

### Trunk-Based Development

**Overview:**  
Trunk-Based Development involves working directly on a single branch (often `trunk` or `main`). Developers integrate changes frequently, often multiple times a day, relying heavily on automated testing and feature toggles to maintain stability.

![Trunk-Based Development](/img/trunk-based.png)

**Resources:**
- [Trunk-Based Development Guide](https://trunkbaseddevelopment.com/)  
- [Martin Fowler – Trunk-Based Development](https://martinfowler.com/articles/continuousIntegration.html)

**Strengths**
- Encourages continuous integration and frequent commits.  
- Reduces merge conflicts by integrating changes quickly.  
- Keeps codebase always releasable with strong CI/CD practices.  
- Promotes collaboration and communication among team members.

**Weaknesses**
- Higher risk of instability if changes are not properly tested.  
- Requires robust CI/CD pipelines and automated testing.  
- Demands discipline to avoid breaking the main branch.  
- Challenging for distributed or less experienced teams.  

## Options Considered

| Workflow    | Complexity | Team Fit | CI/CD Integration | Release Management |
|-------------|------------|----------|-------------------|--------------------|
| Git Flow    | High       | Medium   | Medium            | High               |
| GitHub Flow | Low        | High     | High              | Medium             |
| Trunk-Based | Medium     | Medium   | High              | Low                |

We considered all three workflows against our project’s **team size, development pace, release requirements, and CI/CD capabilities**. Git Flow was ruled out due to its complexity and overhead, while Trunk-Based Development posed potential instability risks without extensive automated testing.

## Our Choice: GitHub Flow

After evaluation, we chose **GitHub Flow** for our project. The key reasons are:

- **Agility and Speed** – Enables rapid iteration and delivery of features.  
- **Collaboration** – Pull requests facilitate code review, knowledge sharing, and peer feedback.  
- **Lightweight** – Minimal branching overhead fits our team’s size and workflow.  
- **CI/CD Friendly** – Seamlessly integrates with continuous integration and deployment pipelines.

**Conclusion:**  
While Git itself is neutral, adopting GitHub Flow introduces the opinionation necessary to bring clarity, structure, and efficiency to our development workflow. It balances the need for rapid delivery, collaboration, and maintainable code, aligning well with our project objectives.

**References:**
1. Vincent Driessen, *A Successful Git Branching Model*, 2010.  
2. GitHub Docs, *GitHub Flow*, [https://docs.github.com/en/get-started/quickstart/github-flow](https://docs.github.com/en/get-started/quickstart/github-flow)  
3. Trunk-Based Development, [https://trunkbaseddevelopment.com](https://trunkbaseddevelopment.com)  
4. Martin Fowler, *Continuous Integration*, [https://martinfowler.com/articles/continuousIntegration.html](https://martinfowler.com/articles/continuousIntegration.html)
