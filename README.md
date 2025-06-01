# Playwright + DevOps

This project is for learn how to run Playwright end-to-end tests with DevOps practices using **Docker** and **GitHub Actions** for continuous integration.

## 🚀 Features

- End-to-end tests using Playwright with **HTML reports** and **trace viewer** support
- Continuous Integration pipeline with **GitHub Actions**
- Dockerized test environment for consistent and isolated test execution
- Playwright browsers automatically installed inside the Docker container
- Sample tests to get started quickly

## 🧪 Run Tests Locally

1. Install dependencies:

   ```bash
   npm install

   ```

2. Install Playwright browsers (required for running tests locally):

   ```bash
   npx playwright install

   ```

3. Run tests:

   ```bash
   npm test

   ```

4. Open test reports (if configured in Playwright config):

   ```bash
   npx playwright show-report
   ```

## 🐳 Run Tests in Docker

1. Build the Docker image:

   ```bash
   docker build -t playwright-devops -f docker/Dockerfile .

   ```

2. Run tests inside the Docker container:

   ```bash
   docker run --rm playwright-devops
   ```
