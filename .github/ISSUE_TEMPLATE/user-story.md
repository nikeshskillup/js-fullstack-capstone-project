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

---

## User Story 6 – Implement Gift Details Page

**Label:** icebox

**As a** user
**I need** to view gift details
**So that** I can learn more about a gift before deciding to comment or share

### Details and Assumptions

* Details will include name, description, price, and image
* Data fetched from backend MongoDB

### Acceptance Criteria

```gherkin
Given the Gifts page
When I click on a gift
Then I should be redirected to the Gift Details page with full information
```

---

## User Story 7 – Implement Search Component

**Label:** icebox

**As a** user
**I need** to search for gifts
**So that** I can quickly find items matching my interest

### Details and Assumptions

* Search bar will support keyword filtering
* Backend endpoint will support search queries

### Acceptance Criteria

```gherkin
Given the Gifts page
When I enter a keyword in the search bar
Then the results should display only the matching gifts
```

---

## User Story 8 – Design and Implement Comments Feature

**Label:** icebox

**As a** community member
**I need** to add comments to gifts
**So that** I can share opinions and interact with other users

### Details and Assumptions

* Users must be logged in to comment
* Comments stored in MongoDB with user reference

### Acceptance Criteria

```gherkin
Given a logged-in user
When they post a comment on a gift
Then the comment should appear instantly and persist in the database
```

---

## User Story 9 – Containerize Services and Applications

**Label:** icebox

**As a** DevOps engineer
**I need** to containerize the backend and frontend
**So that** the application can be deployed consistently across environments

### Details and Assumptions

* Use Docker multi-stage builds
* Separate containers for backend, frontend, and MongoDB

### Acceptance Criteria

```gherkin
Given the Docker environment
When I build and run the containers
Then the backend, frontend, and database should start successfully and interact
```

---

## User Story 10 – Deploy Backend and Frontend

**Label:** icebox

**As a** product owner
**I need** the backend and frontend deployed to a cloud platform
**So that** users can access GiftLink online

### Details and Assumptions

* Deployment could be on IBM Cloud, AWS, or other providers
* CI/CD pipeline preferred

### Acceptance Criteria

```gherkin
Given the deployed environment
When users access the domain
Then they should see the landing page and interact with the backend services
```

---

## Technical Debt Story – Research Authentication in React and Express

**Label:** technical debt

**As a** developer
**I need** to research how authentication works in React and Express
**So that** I can implement a secure login flow

### Details and Assumptions

* Research includes JWT, cookies, and session handling
* Not directly visible to end-users but essential for security

### Acceptance Criteria

```gherkin
Given the need for authentication
When I complete research
Then I should document findings and share them with the team
```
