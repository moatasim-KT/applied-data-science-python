# Setup Guide: Python for Data Science Infrastructure

This guide details how to configure the environment for instructors and students to effectively use this repository.

## 1. Quarto Website Setup
To render and preview the course documentation website:
1. [Download and install Quarto](https://quarto.org/docs/get-started/).
2. In your terminal, navigate to the `course_website/` directory.
3. Run `quarto preview` to start a local development server.
4. The website will be rendered at `http://localhost:XXXX/`.

## 2. GitHub Classroom Setup
To use this repository as a template for student assignments:
1. Go to [GitHub Classroom](https://classroom.github.com/).
2. Create a new classroom.
3. Create a new assignment.
4. Select this repository as the **template repository**.
5. GitHub will automatically create a new repository for each student based on this structure when they accept the assignment.

## 3. CI/CD Pipeline
- **Testing**: Every push to the main branch automatically triggers the `Run Tests` workflow (`.github/workflows/test.yml`), which installs dependencies and runs `pytest`.
- **Deployment**: Any push to the `main` branch that modifies files in `course_website/` triggers the `Deploy Course Website` workflow, which renders the site using Quarto and deploys it to GitHub Pages.

## 4. Development Environment
- **Docker**: For a consistent, reproducible environment, use the provided Dockerfile:
  ```bash
  docker build -t ds-course .
  docker run -p 8888:8888 ds-course
  ```
- **Pre-commit**: To ensure code quality standards, install pre-commit hooks:
  ```bash
  pip install pre-commit
  pre-commit install
  ```
