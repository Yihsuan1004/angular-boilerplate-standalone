# angular-boilerplate-standalone

- [angular-boilerplate-standalone](#angular-boilerplate-standalone)
  - [I、Project Description](#iproject-description)
    - [Features](#features)
  - [II、Project Environment and Packages](#iiproject-environment-and-packages)
    - [Environment Setup](#environment-setup)
    - [VScode Extension Installation](#vscode-extension-installation)
  - [III、Project Startup](#iiiproject-startup)
  - [IV、Project Commit](#ivproject-commit)
  - [V、Commands](#vcommands)
  - [VI、 Project Folder Structure](#vi-project-folder-structure)

## I、Project Description

This is a template project based on the [Angular 16](https://blog.angular.io/angular-v16-is-here-4d7a28ec680d?gi=442df58f98ce) framework, structured as [Standalone](https://angular.io/guide/standalone-components) ; in conjunction with`Google`'s [gts](https://github.com/google/gts), it provides a unified standard and check for the project's code and formatting.

[![Code Style: Google](https://img.shields.io/badge/code%20style-google-blueviolet.svg)](https://github.com/google/gts)

### Features

1. [Commitizen](https://github.com/commitizen/cz-cli) and [Prettier](https://prettier.io/): Utilizes tools for code and commit message formatting.
2. Uses [Google Code Style](https://github.com/google/gts)
3. [Commitlint](https://github.com/conventional-changelog/commitlint) and [ESlint](https://eslint.org/): During commit, syntax checks and enforced formatting are performed to ensure consistency in each submission.
4. Complemented with the use of VScode Extension for automatic formatting and Linting upon file saving.

## II、Project Environment and Packages

### Environment Setup

| tools                                        | version              |
| -------------------------------------------- | -------------------- |
| [Node.js](https://nodejs.org/zh-tw/download) | ^16.14.0 or ^18.10.0 |
| [git](https://git-scm.com/downloads)         | LTS                  |
| [Angular cli](https://angular.io/cli)        | ^16.1.0              |

### VScode Extension Installation

![image-1](./src/assets/pic-1.png)  
Search for `@recommended` within `EXTENSIONS` (as shown in the image above), and you will see the Extensions recommended for installation. Please install all of them.

## III、Project Startup

Enter the following command to install the packages:

```bash
npm install
```

After the packages are installed, enter the following command to start the project:

```bash
ng serve
```

## IV、Project Commit

Enter the following command to invoke the `Commitizen` tool to assist in writing commit messages:

```bash
npm run commit
```

## V、Commands

- `ng serve` - Start the development server.
- `ng build` - Generate the build package.
- `ng test` - Run unit tests.
- `npm run lint` - Execute code checks.
- `npm run commit`- Use Commitizen to submit changes.

## VI、 Project Folder Structure

```text

- 📂 angular-boilerplate-standalone
  - 📂 .angular
  - 📂 .vscode (VSCode Settings)
  - 📂 .husky (Husky Configuration)
  - 📂 e2e
  - 📂 node_modules (Dependencies)
  - 📂 src
      - 📂 app
          - 📂 core (Shared Utility Modules)
               - 📂 enums (Enumeration Declarations)
                   - 📄 common.enum.ts
               - 📂 guards (Route Guards)
               - 📂 utils (Helper Tools)
                   - 📄 common-utils.ts
               - 📂 consts (Constant Declarations)
                   - 📄 common.consts.ts
               - 📂 models (Common Data Models)
                   - 📄 a.model.ts
                   - 📄 b.model.ts
               - 📂 services (Common Services: e.g., Storage)
               - 📂 validators (Validators)
               - 📂 interceptors
          - 📂 features (Feature Modules)
               - 📂 feature-a
                    - 📄 feature-a.component.html
                    - 📄 feature-a.component.scss
                    - 📄 feature-a.component.ts
                    - 📄 feature-a.component.spec.ts
                    - 📂 models (Data Models used by the feature)
          - 📂 shared (Shared Components)
               - 📂 components (Common Components, e.g., dialog, toast)
               - 📂 pipes
               - 📂 directives
               - 📂 layout (Layout Components, e.g., header, navbar)
          - 📄 app.component.html
          - 📄 app.component.scss
          - 📄 app.component.ts
          - 📄 app.module.ts
          - 📄 app.routing-module.ts
     - 📂 assets (Static Resources)
         - 📂 images (Images)
         - 📂 data (Mock API Data)
         - 📂 scripts (External JS)
         - 📂 icons 🔸
     - 📂 styles (Style Files)
          - 📄 _custom.scss 🔸 (Styles for External Packages)
          - 📄 styles.scss
     - 📂 environments (Environment Variables)
          - 📄 environment.ts
          - 📄 environment.prod.ts
     - 📄 index.html
     - 📄 main.ts
     - 📄 polyfills.ts
  - 📄 .eslintrc.json
  - 📄 .eslintignore.json
  - 📄 .lintstagedrc.json
  - 📄 .gitignore
  - 📄 .commitlint.config.js
  - 📄 angular.json
  - 📄 package.json
  - 📄 tsconfig.json
  - 📄 README.md
```
