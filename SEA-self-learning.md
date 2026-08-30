# Self-Learning Activity: Agile, DevOps & Requirement Engineering

## A Case Study Based on a College Canteen Management System

**Subject:** Software Engineering / Software Project Management

**Self-Learning Topic:** Agile, DevOps, JIRA and Requirement Engineering

---

## Introduction

Agile, DevOps, project management tools, and requirement engineering techniques are important parts of modern software development. This self-learning activity studies Agile vs DevOps, JIRA and Asana, user stories and acceptance criteria, advanced requirement elicitation, Requirement Traceability Matrix (RTM), and requirement management tools. A College Canteen Management System is used as a consistent practical context to understand how these concepts can be applied.

---

# 1. Comparison of Agile vs DevOps

Agile focuses on iterative development, customer feedback, and adapting to changing requirements. DevOps focuses on connecting development and operations and improving the build, test, deployment, and monitoring process.

| Aspect | Agile | DevOps |
|---|---|---|
| Main Focus | Iterative development and changing requirements | Continuous delivery and operations |
| Goal | Deliver useful software in small increments | Deliver and maintain software quickly and reliably |
| Teams | Developers, Product Owner, Scrum Master, stakeholders | Development, Operations, QA, Security and related teams |
| Practices | Sprints, backlog, stand-ups, reviews, retrospectives | CI/CD, automation, testing, monitoring |
| Feedback | Customer and stakeholder feedback | Customer and production feedback |
| Release | Frequent releases through iterations | Frequent and increasingly automated releases |
| Common Tools | JIRA, Trello, Azure Boards | Jenkins, Docker, Kubernetes, AWS services |

### How They Work Together

For the canteen system, Agile can divide development into sprints such as login, menu, ordering, and payment. DevOps practices can then automate testing, deployment, and monitoring.

Agile therefore helps organize development, while DevOps improves software delivery and operation.

---

# 2. Case Study: JIRA vs Asana in Real Projects

JIRA is widely used for software development and Agile project management. Asana is a general work and project management platform. Both can organize project work, but their strengths differ.

| Feature | JIRA | Asana |
|---|---|---|
| Primary Use | Software development and Agile management | General project and task management |
| Work Items | Issues, stories, bugs, tasks, epics | Tasks and subtasks |
| Scrum | Strong support | Not a core focus |
| Bug Tracking | Strong | Not its primary purpose |
| Backlog | Supported | Not centered on a traditional development backlog |
| Reporting | Agile and development-focused | Progress, workload and timeline views |
| Best Fit | Software/product teams | Cross-functional teams |

## Case Example

In the College Canteen Management System, a JIRA Epic could be **“Online Food Ordering”**.

Stories can include:

- Viewing the menu
- Adding items to a cart
- Placing an order
- Making payment
- Checking order status

Issues can move through:

**Backlog → To Do → In Progress → Testing → Done**

The same project could be managed in Asana through tasks such as:

- Designing the menu screen
- Creating the food database
- Implementing payment
- Testing the order process
- Preparing documentation

JIRA is generally stronger when the project needs Agile development workflows, while Asana is convenient for general task coordination.

---

# 3. Writing Effective User Stories and Acceptance Criteria

A user story expresses a requirement from the perspective of the person who will use the system.

A common format is:

> **As a [user], I want [goal], so that [benefit].**

## Example

> **As a student, I want to place a food order before reaching the canteen, so that I can reduce my waiting time.**

The INVEST principles for a good user story are:

- **Independent**
- **Negotiable**
- **Valuable**
- **Estimable**
- **Small**
- **Testable**

## Additional Examples

- As a student, I want to log in using my college credentials, so that I can securely access my account.
- As a student, I want to view today's menu and prices, so that I can decide what to order.
- As a student, I want to see my order status, so that I know when my food will be ready.

## Acceptance Criteria

Acceptance criteria define the conditions that must be satisfied for a user story to be complete.

### Example Acceptance Criteria for Online Ordering

1. Student can select available food items.
2. Selected items appear in the cart.
3. Total price is calculated correctly.
4. Student can confirm the order.
5. A unique order number is generated.
6. Student can view the order status.

## Given–When–Then

> **Given** the student has selected food items,  
> **When** the student confirms the order and completes payment,  
> **Then** the system should create the order and display the order number.

---

# 4. Advanced Requirement Elicitation Techniques

Requirement elicitation is the process of discovering, understanding, and documenting the needs of users and other stakeholders.

## a) Interviews

Analysts can interview students, canteen staff, and administrators to understand problems with the existing process. Interviews may be:

- Structured
- Semi-structured
- Unstructured

## b) Ethnography

The analyst observes users in their real environment.

Observing the canteen during lunch may reveal:

- Long queues
- Repeated manual order-taking
- Billing delays
- Difficulty identifying completed orders

## c) Prototyping

An early model of the system can include:

- Login
- Menu
- Cart
- Payment
- Order-status screens

Users can review the prototype and suggest changes before development.

## d) JAD — Joint Application Development

Joint Application Development brings stakeholders together in structured sessions to discuss requirements and resolve differences.

## e) Focus Groups

A selected group of students can discuss:

- Ordering preferences
- Payment methods
- Notifications
- Problems with the current process

## f) Document Analysis

Existing:

- Menus
- Price lists
- Billing records
- Forms
- College rules

can be studied to identify requirements and constraints.

## Requirement Elicitation Technique Comparison

| Technique | Main Idea | Canteen Example |
|---|---|---|
| Interview | Ask stakeholders directly | Interview students and staff |
| Ethnography | Observe users in context | Observe lunch-hour queues |
| Prototyping | Show an early model | Create ordering-screen prototype |
| JAD | Collaborative stakeholder session | Students + staff + administration |
| Focus Group | Discuss with selected users | Discuss features with students |
| Document Analysis | Study existing records | Analyze menu and billing records |

---

# 5. Requirement Traceability Matrix (RTM)

A Requirement Traceability Matrix connects individual requirements with related design and testing activities. It helps ensure that important requirements are not missed and can be verified.

## Purpose

RTM can be used to:

- Track requirements
- Connect requirements with test cases
- Identify gaps
- Understand changes
- Improve testing coverage
- Maintain documentation

## Example RTM: College Canteen Management System

| Req ID | Requirement | Source | Design Reference | Test Case | Status |
|---|---|---|---|---|---|
| REQ-001 | Student can register | Student | User Module | TC-001 | Passed |
| REQ-002 | Student can log in | Student | Authentication | TC-002 | Passed |
| REQ-003 | Student can view menu | Student | Menu Module | TC-003 | Passed |
| REQ-004 | Student can add items to cart | Student | Cart Module | TC-004 | In Progress |
| REQ-005 | Student can place order | Student | Order Module | TC-005 | In Progress |
| REQ-006 | Student can view order status | Student | Tracking Module | TC-006 | Not Started |

## Types of Traceability

### Forward Traceability

**Requirement → Design → Test Case**

It checks whether requirements are carried into development and testing.

### Backward Traceability

**Test Case → Requirement**

It checks whether test cases correspond to valid requirements.

### Bi-directional Traceability

**Requirement ↔ Design ↔ Test Case**

It provides visibility in both directions.

---

# 6. Tools for Requirement Management

Requirement management tools help teams capture, organize, update, track, and trace requirements throughout the software lifecycle.

| Tool | Description | Best Used For |
|---|---|---|
| IBM DOORS | Requirements management and traceability | Large and complex projects |
| JIRA | Stories, tasks, bugs and project work | Agile software development |
| Confluence | Collaborative documentation | Project and requirement documentation |
| Polarion ALM | Requirements and lifecycle management | Enterprise projects |
| Visure Requirements | Requirements, traceability and risk management | Compliance-oriented projects |
| Excel / Google Sheets | Simple manual requirement tracking | Small projects |

## IBM DOORS

IBM DOORS is a specialized requirements management solution for capturing, organizing, linking, and tracing requirements.

It can be useful where requirements require strong control and traceability.

## JIRA

JIRA can manage:

- Epics
- User stories
- Tasks
- Bugs
- Development work

It is useful for Agile teams.

## Confluence

Confluence supports collaborative documentation such as:

- Requirements
- Meeting notes
- Technical documentation
- Project knowledge

## Polarion ALM

Polarion ALM supports requirements and application lifecycle management and can connect requirements, development, and testing activities.

## Visure Requirements

Visure Requirements supports:

- Requirements
- Traceability
- Risk management
- Compliance-related information

## Excel / Google Sheets

Excel and Google Sheets are simple and accessible for small projects and RTMs, but require more manual management than specialized platforms.

---

# Conclusion

Agile, DevOps, project management tools, and requirement engineering techniques support different but connected parts of modern software development. Agile helps teams work iteratively and respond to changing requirements, while DevOps improves continuous delivery and operations.

JIRA and Asana help organize project work for different types of teams. User stories and acceptance criteria make requirements clearer and testable.

Requirement elicitation techniques help uncover stakeholder needs, while RTM connects requirements with design and testing.

Tools such as IBM DOORS, JIRA, Confluence, Polarion, Visure, and spreadsheets support requirement management at different levels of complexity.

The College Canteen Management System demonstrates how these concepts can be applied together in a practical project.

---

# References

1. AWS — What is DevOps?  
   https://aws.amazon.com/devops/what-is-devops

2. Atlassian — JIRA Software  
   https://www.atlassian.com/software/jira

3. Asana — Project Management  
   https://asana.com/

4. IBM — IBM Engineering Requirements Management DOORS  
   https://www.ibm.com/products/requirements-management-doors

5. Agile Manifesto  
   https://agilemanifesto.org/
