---
sidebar_position: 4
sidebar_label: Technology Stack
---

# Technology Stack

Selecting the right technology stack is crucial for building maintainable, scalable, and performant applications. The stack defines the programming languages, frameworks, libraries, and services used to develop, deploy, and operate the software. We evaluated multiple options for frontend, backend, database, and authentication to identify a combination that balances performance, developer productivity, and long-term sustainability.

### Backend Frameworks

#### Node.js

**Overview:**  
Node.js is a **JavaScript runtime environment** built on Chrome's V8 engine that enables server-side scripting.


**Strengths**
- High performance due to non-blocking, event-driven architecture.  
- Large ecosystem with npm packages for almost any functionality.  
- Unified language for frontend and backend (JavaScript).  
- Suitable for building scalable APIs and real-time applications.

**Weaknesses**
- Single-threaded nature can be limiting for CPU-intensive tasks.  
- Callback-heavy code can become complex, though modern async/await mitigates this.  
- Requires careful error handling to maintain server stability.

#### Express.js

**Overview:**  
Express.js is a **lightweight web application framework** for Node.js, simplifying routing, middleware integration, and HTTP handling.


**Strengths**
- Minimalistic and flexible, allowing developers to structure applications as needed.  
- Large community and extensive middleware ecosystem.  
- Simplifies RESTful API development.  
- Lightweight and performant.

**Weaknesses**
- Lacks opinionated structure; developers must enforce best practices themselves.  
- Scaling very large applications may require additional architectural patterns.  
- Limited built-in security; developers must handle authentication and protection carefully.

### Frontend Technologies

#### React

**Overview:**  
React is a **JavaScript library** for building user interfaces using components and declarative rendering.


**Strengths**
- Component-based architecture promotes reusable, maintainable code.  
- Virtual DOM improves rendering performance.  
- Large ecosystem and community support.  
- Excellent for building dynamic, interactive UIs.

**Weaknesses**
- Requires learning JSX and component lifecycle concepts.  
- State management can become complex in large applications without proper patterns (e.g., Redux, Context API).  
- SEO for client-rendered apps requires additional configuration or server-side rendering.

#### CSS

**Overview:**  
CSS (Cascading Style Sheets) is used for **styling web applications**, controlling layout, colours, fonts, and responsiveness.

**Strengths**
- Widely supported and essential for web UI development.  
- Flexible and powerful, especially with preprocessors (Sass, Less) or frameworks (Tailwind, Bootstrap).  
- Enables responsive and adaptive designs.

**Weaknesses**
- Can become hard to maintain in large projects without conventions.  
- Browser inconsistencies may require additional testing and fixes.  
- Advanced layouts may require additional tooling.

### Database and Authentication

#### PostgreSQL

**Overview:**  
PostgreSQL is an **open-source relational database** known for reliability, standards compliance, and powerful features.

**Strengths**
- Strong support for complex queries, transactions, and data integrity.  
- Extensible with custom functions, data types, and indexing.  
- Active community and widely used in production.  
- ACID-compliant, suitable for critical applications.

**Weaknesses**
- Requires schema planning and maintenance.  
- Performance tuning can be complex for very large datasets.  
- Learning curve for advanced features (e.g., stored procedures, triggers).

#### Firebase Authentication

**Overview:**  
Firebase Authentication is a **cloud-based service** providing secure user authentication and identity management.

**Strengths**
- Simplifies implementing email/password, social login, and multi-factor authentication.  
- Integrated with Firebase ecosystem (Firestore, Realtime Database).  
- Handles security and token management out-of-the-box.  
- Reduces backend complexity for authentication.

**Weaknesses**
- Vendor lock-in; switching providers can be challenging.  
- Limited customisation of authentication flows.  
- Dependent on external service uptime and internet connectivity.

## Our Choice: Express.js + Node.js + React + CSS + PostgreSQL + Firebase Authentication

**Reasons for this choice**
- **Performance and Scalability** – Node.js and Express.js provide a fast, lightweight backend.  
- **Component-based Frontend** – React enables modular, maintainable UI development.  
- **Data Reliability** – PostgreSQL ensures strong data integrity and support for complex queries.  
- **Rapid Development and User Management** – Firebase Authentication simplifies secure login and reduces backend complexity.  
- **Maintainability and Standardisation** – CSS ensures consistent styling across the application.

**Conclusion:**  
This technology stack allows the team to **build a scalable, maintainable, and high-performance application** while leveraging widely adopted, community-supported tools and frameworks.

**References:**
1. Node.js, [https://nodejs.org](https://nodejs.org)  
2. Express.js, [https://expressjs.com](https://expressjs.com)  
3. React, [https://reactjs.org](https://reactjs.org)  
4. PostgreSQL, [https://www.postgresql.org](https://www.postgresql.org)  
5. Firebase Authentication, [https://firebase.google.com/docs/auth](https://firebase.google.com/docs/auth)