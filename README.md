# Account Management Fullstack: Screening

**Before you get started, please read [this guide](https://www.notion.so/Get-started-with-your-assignment-dade100d93054a6db1036ce294bdaeb6)** that walks you through how to submit your solution and get help.

### Estimated time investment ⏳

- Completing the task: **1 hour**
- Configuring the remote tests: **15 minutes**

### The challenge 🎯

Your task is to build a Fullstack app that integrates and implements this [API specification](api-specification.yml). The API defines a set of operations for creating and reading account transactions. You can use [editor.swagger.io](https://editor.swagger.io/) to visualize the spec.

#### Frontend mockup 🧱
<img src="https://github.com/DevSkillsHQ/am-fullstack-screening/blob/main/mockup.png?raw=true" height="550">
 
#### Frontend specification 📘
* There's a form with two input fields: Account ID and Amount. Whenever the form is submitted, a new transaction with the collected data should be created on the backend, and the corresponding input fields are cleared. The HTML elements must have the following HTML attributes:
  * Account ID input field: `data-type="account-id"`
  * Amount input field: `data-type="amount"`
  * Form: `data-type="transaction-form"`
* There's a list of the previously submitted transactions. Every newly submitted transaction should appear at the top of the list. The HTML element that represents a transaction should include the following HTML attributes: `data-type=transaction`, `data-account-id={transaction-account-id}`, `data-amount={transaction-amount}`, and `data-balance={current-account-balance}`

### The focus areas 🔍

#### Backend
- **Use a SQLite database as the service datastore.** We want to see how you design your database schema and SQL queries for working with the service data. Pleae use [SQLite](https://www.sqlite.org/index.html) as it doesn't require running a DB server, which simplifies running the tests in the pipeline.
- **Create a backend service that implements the provided API.** Make sure all predefined API tests pass. It will involve the following:
  - Handling invalid HTTP requests;
  - Creating new transactions;
  - Fetching the current account balance;

#### Frontend
- **Integrate with a REST API**. Using the provided API spec, figure out the right service endpoints to use.

### The provided boilerplate 🗂
* The [service specification](api-specification.yml) in the Open API format.
* Automated tests to validate your solution. To run locally:
  * Install the required test dependencies with `npm install` (please give it some time to download the necessary dependencies).
  * Update the `baseUrl` (where your Frontend will run) and the `apiUrl` (where your Backend will run) in [cypress.json](cypress.json).
  * Run your Fullstack app.
  * Run the tests with `npm run test`. Alternatively, Backend tests only: `npm run test:backend` or Frontend tests only: `npm run test:frontend`.

### Before submitting your solution ⚠️
1. Update the `baseUrl` (where your Frontend will run) and the `apiUrl` (where your Backend will run) in [cypress.json](cypress.json).
2. Update the [`build:fullstack`](package.json#L5) and [`start:fullstack`](package.json#L6) scripts in [package.json](package.json) that respectively build and run your application. **[See examples](https://www.notion.so/devskills/Fullstack-991deeab9622416389fd2fd9fb41da85)**.

---

Made by [DevSkills](https://devskills.co). 

How was your experience? **Give us a shout on [Twitter](https://twitter.com/DevSkillsHQ) / [LinkedIn](https://www.linkedin.com/company/devskills)**.
