# **Final Project: Git Collaboration Simulation**

You will work with a partner to simulate a mini software development project using Git. The focus is on collaboration, branch management, conflict resolution, and proper Git history practices.
  
The first thing to do is for one team member to **fork** this repository. This will serve as your team’s **Starter Repository**.

## **Setup Instructions**

1. **Clone the Starter Repository**

```shell
git clone <repo-url>
cd pseudo-shop
```

2. **Create Your Own Feature Branch** Each person must create a feature branch for their assigned tickets:

```shell
git checkout -b feat/<feature-name>
```

3. **Coordinate With Your Partner** Decide who works on which features. Communicate regularly to avoid duplicate work.

## **Your Goals**

Complete and commit code for all of the following features:

1. Filter products by attributes (width, height, etc.)  
2. User registration and login  
3. Product creation and listing  
4. Storefront display logic

## **Git Workflow Requirements**

* Use feature branches. No one should commit directly to `main`.  
* Each feature must have at least **3 commits** with clear messages.  
* Push your branches to GitHub:

```shell
git push origin feat/<feature-name>
```

* Use `git merge` to integrate into `main` once a feature is complete.  
* At least one **merge conflict** must be experienced and resolved.  
* Use `git log` to review your history before final submission.

## **Deliverables**

1. **Final GitHub Repo**  
     
   * Must show all feature branches and a clean `main` branch with merged work

   

2. **Retrospective File (`retrospective.md`)**  
     
   * Answer all reflection questions in the template

   

3. **Implemented Features**  
     
   * All four features must be coded using the provided `.pseudo` files

## **Due Date and Submission**

Refer to your activity document.

---

## Code Style Guide:

* Variable names: `snake_case`  
* Function names: `snake_case`  
* Class names: `CamelCase`  
* No import system needed; assume all files are magically available

---

## Feature Tickets

### **Feature 1: Filter Products by Attributes**

**Title:** `[Feature] Filter by product attributes`

**Description:** Allow users to filter products based on width, height, length, weight, color, and brand.

**Exit Criteria:**

* A function `filter_products(filters)` exists  
* Filtering can be demonstrated in the `store_view.pseudo` file  
* Product data in `product_model.pseudo` includes all needed attributes

### **Feature 2: User Registration and Login**

**Title:** `[Feature] User registration and login`

**Description:** Implement user creation with basic login functionality using pseudo-credentials.

**Exit Criteria:**

* Function `create_user(name, email, password)` is defined in `user_controller.pseudo`  
* Function `login_user(email, password)` returns success/failure  
* User data is stored in a list or simple in-memory structure

### **Feature 3: Product Management**

**Title:** `[Feature] Product creation and listing`

**Description:** Add capability to create products and view the full list of available items.

**Exit Criteria:**

* Function `add_product(...)` adds a product to a list  
* `product_model.pseudo` contains a working in-memory data structure  
* `store_view.pseudo` can render the full list of products

### **Feature 4: Display Storefront**

**Title:** `[Feature] Storefront layout and display logic`

**Description:** Design the store interface and show all product information in a structured format.

**Exit Criteria:**

* Function `display_products()` exists  
* Output shows name, price, and filtered attributes  
* Follows pseudo-code style guide

---

## Define Git Workflow Rules

### Git Workflow Requirements

**1\. Branch Naming Convention**

* Feature branches must follow: `feat/<feature-name>`   
  Example: `feat/user-auth`, `feat/filter-products`

**2\. Progressive Commits**

* Each student must make at least 3 commits per feature  
* Commit messages must be descriptive (e.g., `Add login function`, not `stuff`)

**3\. Pushing to Remote**

* Students must push all feature branches to GitHub  
* No work should be done directly on `main`

**4\. Pull Requests (Optional if not using GitHub PRs)**

* If using GitHub PRs: teams must open PRs before merging  
* If not: simulate PR by reviewing and discussing before merging

**5\. Merging to Main**

* Merge completed features into `main` only after:  
    
  * Work is complete  
  * Merge conflicts (if any) are resolved  
  * Both partners agree

**6\. Conflict Resolution Requirement**

* At least one **intentional merge conflict** must occur during the project (e.g., both modify the same function or line)  
    
* Students must document:  
    
  * What caused the conflict  
  * How they resolved it

**7\. Final State**

* All branches merged to `main`  
* No orphaned or unpushed branches  
* Git history must reflect progressive work and collaboration

---

## Simulate Team Collaboration Guidelines

### Team Setup

* Teams of **two**  
* Both clone the same starter repository  
* Both must contribute code and Git history

### Collaboration Expectations

**1\. Workload Division**

* Teams are responsible for dividing the four feature tickets between them  
* Division should consider interdependencies (e.g., product creation needed before filtering)

**2\. Communication**

* Teams must coordinate:  
    
  * Who starts which feature  
  * When to merge  
  * How to resolve conflicts (e.g., using VS Code live share or Zoom calls)

**3\. Conflict Simulation**

* At least one conflict must be **intentional** Example: both edit the `display_products()` function in `store_view.pseudo`  
* Teams must resolve it collaboratively (no force-push or overwrite)

**4\. Commit Hygiene**

* Avoid dumping all changes in one commit  
* Make sure both team members have visible contributions (use `git log` or GitHub contributors tab)

### Suggested Tools for Communication (not required)

* GitHub Issues for tracking features  
* Commenting on PRs  
* Shared notes or docs for planning

---

## Student Submission Requirements


### 1\. **Final GitHub Repository Link**

* Must be pushed to GitHub under one team member’s account (can be private or public)  
* All feature branches must be visible in the repository  
* `main` branch should include all merged features

### 2\. **Retrospective Report (`retrospective.md`)**

Each team must submit a reflection report in markdown format, included in the root of the repo. This file should answer the following questions:

**Required Questions:**

1. How did your team divide the work?  
2. What Git commands or workflows were most useful to you?  
3. Describe the merge conflict your team encountered. What caused it and how did you resolve it?  
4. What were the biggest challenges during this activity?  
5. What did you learn about using Git in a team setting?  
6. How would you improve your workflow in future projects?

### 3\. **Git History Quality**

* Git log should show:  
    
  * Progressive commits  
  * Multiple contributors  
  * Merges and resolved conflicts


* No "squash and merge" or rewriting history allowed

### 4\. **Code Consistency**

* Follow the pseudo-code and style guide from the README  
* Files must be clean, organized, and syntactically consistent

### 5\. **Feature Completion**

Each of the four features must be:

* Implemented in pseudo-code  
* Satisfy the exit criteria stated in the ticket  
* Testable via reading the `.pseudo` files (e.g., does `display_products()` print values?)


