---
sidebar_position: 6
sidebar_label: Source Code Management
---

# Source Code Management

Effective source code management (SCM) and maintenance are crucial for ensuring code quality, consistency, and collaboration across the development team. SCM involves tracking changes, managing versions, and enabling multiple developers to work on the same codebase without conflicts. Maintenance focuses on keeping the codebase clean, well-documented, and scalable over time.

To ensure effective collaboration and maintain code quality, our team evaluated several tools and practices for SCM, source control platforms, and code quality enforcement. Below we document the options considered, their strengths and weaknesses, and the rationale for our chosen approach.

### Git

**Overview:**  
Git is a **distributed version control system** widely used for modern software projects. It enables branching, merging, and offline work while maintaining a complete history of the repository.


**Resources:**
- [Git Documentation](https://git-scm.com/doc)  
- [Atlassian – Git Basics](https://www.atlassian.com/git/tutorials/what-is-version-control)

**Strengths**
- Distributed – every developer has a full copy of the repository.  
- Supports branching and merging for parallel development.  
- Powerful history and rollback features.  
- Large community and tool integrations.

**Weaknesses**
- Can be complex for beginners, especially when resolving conflicts.  
- Requires disciplined workflow to maintain code quality.

### Subversion (SVN)

**Overview:**  
SVN is a **centralised version control system** with a single repository serving as the source of truth.


**Resources:**
- [SVN Book](https://svnbook.red-bean.com/)

**Strengths**
- Easier learning curve for beginners due to linear workflow.  
- Centralised repository ensures a single source of truth.

**Weaknesses**
- Less flexible for branching and merging.  
- Requires network access for most operations.  
- Not ideal for parallel development or offline work.

### Mercurial

**Overview:**  
Mercurial is a **distributed version control system** similar to Git, designed to be simpler to use.


**Resources:**
- [Mercurial Documentation](https://www.mercurial-scm.org/)

**Strengths**
- Simple command set; easier learning curve than Git.  
- Distributed, allowing offline work.  
- Supports branching and merging.

**Weaknesses**
- Smaller community and fewer integrations.  
- Less widely adopted, limiting available resources.

### Git Server Platforms

Choosing the right platform for hosting repositories and facilitating collaboration is critical. These platforms provide pull requests, code reviews, issue tracking, and CI/CD integration.


#### GitHub

**Overview:**  
GitHub is a **cloud-based Git platform** providing repository hosting, collaboration features, and CI/CD integration.


**Resources:**
- [GitHub Docs](https://docs.github.com/)

**Strengths**
- Integrated task management linking code, issues, and tasks.  
- Supports pull requests and code reviews.  
- CI/CD and automated testing integrations.

**Weaknesses**
- Public repositories may expose code if not configured.  
- Some advanced features require paid plans.  
- Requires disciplined workflows.

#### GitLab

**Overview:**  
GitLab is a **repository management platform** with integrated CI/CD and DevOps tools.


**Resources:**
- [GitLab Docs](https://docs.gitlab.com/)

**Strengths**
- Comprehensive platform including code hosting, CI/CD, and issue tracking.  
- Supports self-hosted or cloud deployment.

**Weaknesses**
- Can be complex to set up and maintain.  
- Feature-rich interface may be overwhelming for smaller teams.

### Linters and Code Quality Tools

**Overview:**  
Linters automatically check source code for style, formatting, and potential errors, helping enforce team coding standards and maintain code quality.


**Resources:**
- [ESLint](https://eslint.org/)  
- [Prettier](https://prettier.io/)  
- [Stylelint](https://stylelint.io/)

**Strengths**
- Enforces coding standards and reduces early errors.  
- Improves readability and maintainability.  
- Integrates with editors and CI/CD pipelines.

**Weaknesses**
- Requires configuration for project-specific standards.  
- May be perceived as strict if not aligned with team practices.

## Options Considered

| Tool / Platform | Type | Complexity | Collaboration | CI/CD Integration | Learning Curve |
|-----------------|------|------------|---------------|-----------------|----------------|
| Git             | Distributed VCS | Medium | High | High | Medium |
| SVN             | Centralised VCS | Low | Medium | Low | Low |
| Mercurial       | Distributed VCS | Medium | Medium | Medium | Low |
| GitHub          | Cloud Platform  | Low | High | High | Low |
| GitLab          | Cloud/Self-host | Medium | High | High | Medium |
| Linters         | Quality Tools  | Low | Medium | High | Low |

We compared each option against **complexity, collaboration capabilities, CI/CD integration, and learning curve**. Git and GitHub were preferred due to their distributed architecture, strong collaboration features, and CI/CD integration. Linters complement this setup to maintain code quality.

## Our Choice: Git + GitHub + Linters

After evaluation, we selected **Git** as our version control system, **GitHub** as our collaboration platform, and **linters** for code quality.

**Reasons for this choice**
- **Reliable Version Control** – Git provides robust branching, merging, and history tracking.  
- **Integrated and Centralised Task Management** – GitHub links tasks, issues, and code for transparency.  
- **Code Quality and Consistency** – Linters enforce coding standards, reduce errors, and improve maintainability.

**Conclusion:**  
This combination allows our team to **collaborate efficiently, maintain high code quality, and ensure long-term sustainability of the project**.

**References:**
1. Atlassian – Version Control Systems, [https://www.atlassian.com/git/tutorials/what-is-version-control](https://www.atlassian.com/git/tutorials/what-is-version-control)  
2. Git Documentation, [https://git-scm.com/doc](https://git-scm.com/doc)  
3. GitHub Docs, [https://docs.github.com](https://docs.github.com)
