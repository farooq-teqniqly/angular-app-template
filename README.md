# Angular 19 Starter Template

This template gets you up and running with a starter Angular 19 app.

The template is configured with Husky, providing the following benefits:

- **Pre-commit checks on staged files**: When files are committed locally, Husky will:
    - Format the files using [Prettier](https://prettier.io/).
    - Lint the files using [ESLint](https://eslint.org/).
    - If any step fails, the commit is blocked to maintain a high level of code quality.
- **Commit message standardization**: Ensures commit messages adhere to a [standard format](https://commitlint.js.org/concepts/commit-conventions.html) with the help of [commitlint](https://commitlint.js.org/). The default configuration can be customized by editing `commitlint.config.js` in the repository root.

## Running the Template Application

### Prerequisites
- **Node.js**: Ensure Node.js (version 20 or later) is installed.
- **npm**: Ensure npm (version 10 or later) is installed.

### Install Husky Dependencies
Run the following command in the **repository root** to install Husky and its dependencies:

```bash
npm install
```
> Note: Do not install any Angular app-related packages in the root folder.

## Install Angular Application Dependencies
The Angular application files are located in the `todo` directory. Navigate to the `todo` directory and run:
```bash
npm install
```
This will install the application's dependencies.

> Rationale: The root folder contains only dependencies related to Husky, allowing for potential future additions like a backend folder that can also utilize Husky's features.

## Run the Application

To start the application, navigate to the `todo` directory and run:

```bash
ng serve
```
By default, Vite hosts the application at http://localhost:4200.

## Customizing the Configuration

### Husky and commitlint
Modify Husky hooks and commitlint rules by editing the respective configuration files in the
root folder (`.husky/` and `commitlint.config.js`).
