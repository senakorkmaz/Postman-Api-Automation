# Postman API Automation

This repository provides a framework for automating API tests using Postman. It includes collections and environments designed to validate API endpoints effectively.

## Repository Structure

- **collections/**: Contains Postman collection files (.json) that define the API test suites.
- **.github/workflows/**: Includes GitHub Actions workflows for automating test executions.

## Prerequisites

Ensure the following are installed on your system:

- [Node.js](https://nodejs.org/) (version 14 or higher recommended)
- [Newman](https://www.npmjs.com/package/newman) - Postman's command-line collection runner

Install Newman globally using npm:

```sh
npm install -g newman
```

## Running Tests Locally

To execute the tests locally using Newman:

1. Navigate to the repository directory.
2. Run the following command:

```sh
newman run collections/PostmanAutomationCollection.json
```

## Continuous Integration with GitHub Actions

This project utilizes GitHub Actions for continuous integration. The workflow is defined in `.github/workflows/`. It automates the execution of Postman collections on each push or pull request to the repository.