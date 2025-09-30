# GiftLink Project – User Stories

This document captures the user stories for the GiftLink Capstone Project.
Each story is written from the end-user’s perspective and includes details, assumptions, acceptance criteria, and the initial **label assignment**.

---

## User Story 1 – Finish User Stories

**Label:** backlog

**As a** product owner
**I need** to have all required user stories documented and available in GitHub issues
**So that** the development team has clarity on project scope and deliverables

### Details and Assumptions

* All 10 core stories must be created as GitHub issues
* Each story should use the template provided

### Acceptance Criteria

```gherkin
Given the GitHub repository
When I open the Issues tab
Then I should see all project user stories as issues using the defined template
```

---

## User Story 2 – Initialize and Populate MongoDB

**Label:** backlog

**As a** backend developer
**I need** to set up MongoDB and seed it with initial data
**So that** the backend services can store and retrieve gift information

### Details and Assumptions

* MongoDB will run locally or in a container
* Initial dataset will include gifts, users, and comments

### Acceptance Criteria

```gherkin
Given a fresh project environment
When MongoDB is started and seeded
Then collections for users, gifts, and comments should exist with sample data
```

---

## User Story 3 – Run Skeleton Application

**Label:** backlog

**As a** developer
**I need** to run the existing skeleton application
**So that** I can verify the base project setup before enhancements

### Details and Assumptions

* Backend skeleton is provided in the template
* App should compile and start without errors

### Acceptance Criteria

```gherkin
Given the template project
When I run the skeleton application
Then it should start successfully and expose default endpoints
```

---

## User Story 4 – Implement Landing Page and Navigation

**Label:** backlog

**As a** user
**I need** a landing page with navigation links
**So that** I can explore GiftLink’s features easily

### Details and Assumptions

* React frontend will provide Home, Login, Gifts, and About navigation
* Navbar will be consistent across all pages

### Acceptance Criteria

```gherkin
Given the frontend application
When I open the landing page
Then I should see navigation links for Home, Login, Gifts, and About
```

---

## User Story 5 – Add Authentication Components and Logic

**Label:** backlog

**As a** user
**I need** to log in securely
**So that** I can personalize my GiftLink experience

### Details and Assumptions

* Authentication will use JWT
* Login and registration components will exist in React

### Acceptance Criteria

```gherkin
Given a new user
When they register and log in
Then they should receive a valid JWT token and access restricted pages
```

