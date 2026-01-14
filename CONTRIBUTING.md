# Contributing to SpendWise

First off, thank you for considering contributing to SpendWise! We're excited to see what you build. This project is a great place to learn and practice your full-stack development skills.

This document provides guidelines for contributing to the project. Whether you're fixing a bug, adding a new feature, or improving documentation, your help is greatly appreciated.

## Code of Conduct
We have a [Code of Conduct](CODE_OF_CONDUCT.md) to ensure our community is welcoming and inclusive for everyone. Please take a moment to read it before you get started.

## How Can I Contribute?
There are many ways to contribute, from writing code and tests to improving the documentation.

### Reporting Bugs
If you find a bug, please open an issue and provide a clear description, including steps to reproduce it.

### Suggesting Enhancements
Have an idea for a new feature or an improvement to an existing one? Feel free to open an issue to discuss it. We recommend starting a discussion before you spend a lot of time on implementation.




### 3. Create a New Branch
Create a new branch for your feature or bug fix. Use a descriptive name.
```bash
# For a new feature
git checkout -b feature/add-transaction-filters

# For a bug fix
git checkout -b fix/dashboard-chart-bug
```

### 4. Set Up the Project
Follow the instructions in the main README.md file to set up the backend and frontend environments, including installing dependencies and creating your .env files.

### 5. Make Your Changes
Now you're ready to write your code! Make your changes in the relevant files.

### 6. Run Tests
Before you submit your contribution, please make sure all tests are passing.
```bash
# In the /backend directory
npm test

# In the /frontend directory
npm test
```
If you're adding a new feature, please add a corresponding test for it.

### 7. Commit Your Changes
Commit your changes with a clear and descriptive message.
```bash
git add .
git commit -m "feat: Add date range filters to transactions page"
```

- feat: A new feature
- fix: A bug fix
- docs: Changes to documentation
- style: Formatting changes (e.g., whitespace)
- refactor: Code changes that neither fix a bug nor add a feature
- test: Adding or correcting tests

Read more [here](https://www.conventionalcommits.org/en/v1.0.0/) for guidelines on how to write commit messages.

### 8. Push to Your Branch
Push your changes up to your forked repository.
```bash
git push origin feature/add-transaction-filters
```