## Project Readme

This repo is intended to be used a project starter. The project uses the Vite development server for development, testing and previewing. The project has dependencies on React and React DOM libraries and also includes several devDependencies that are essential for development and testing of the project.

### Scripts

The following scripts are included in the project:

- `dev`: Runs the Vite development server.
- `build`: Builds the project using the TypeScript compiler and Vite bundler.
- `preview`: Runs a preview of the production build using the Vite server.

### DevDependencies

The project has several devDependencies, including:

- `@testing-library/jest-dom`: A set of custom jest matchers to test the state of the DOM.
- `@testing-library/react`: A set of utilities for testing React components.
- `@typescript-eslint/eslint-plugin` and `@typescript-eslint/parser`: TypeScript support for ESLint.
- `eslint`, `eslint-config-airbnb`, `eslint-config-airbnb-typescript`, `eslint-config-prettier`, `eslint-plugin-import`, `eslint-plugin-jsx-a11y`, `eslint-plugin-prettier`, `eslint-plugin-react`, `eslint-plugin-react-hooks`: A collection of tools for enforcing coding standards and catching errors in the code.
- `prettier`: A code formatter to keep the code clean and consistent.
- `typescript`: A language for application-scale JavaScript.

### Usage

To use the project, clone the repository and run `npm install` to install all the dependencies. After installation, run `npm run dev` to start the development server. You can then edit the code and the server will automatically reload the changes.

To build the project for production, run `npm run build`. The resulting files will be placed in the `dist` folder. To preview the production build, run `npm run preview`. The Vite server will serve the production files, and you can test the application to make sure everything is working as expected.

### Typescript Options

- `target`: Specifies the ECMAScript target version. In this case, it's set to ESNext, which means the latest version of ECMAScript.

- `useDefineForClassFields`: Enables emitting ECMAScript-standard-compliant class fields.

- `lib`: Specifies the library files to be included in the compilation. This project includes DOM, DOM.Iterable, and ESNext.

- `allowJs`: Allows JavaScript files to be included in the compilation.

- `skipLibCheck`: Skips type checking of all declaration files.

- `esModuleInterop`: Enables compatibility with ES modules.

- `allowSyntheticDefaultImports`: Allows default imports from modules with no default export.

- `strict`: Enables all strict type-checking options.

- `forceConsistentCasingInFileNames`: Ensures that all referenced files and directories are addressed with the same casing.

- `module`: Specifies the module system used. This project uses ESNext modules.

- `moduleResolution`: Specifies how modules are resolved. This project uses Node's module resolution algorithm.

- `resolveJsonModule`: Enables importing JSON files as modules.

- `isolatedModules`: Disables emitting files that are not explicitly specified on the command line.

- `noEmit`: Disables emitting files from TypeScript compilation.

- `jsx`: Specifies the JSX factory function. This project uses the `react-jsx` option.

### Eslint Options

- `env`: An object that defines the global variables that are available during the execution of a program. This project specifies that the browser and ECMAScript 2021 (ES12) are enabled.

- `extends`: An array of configurations that extend the base configuration. This project extends the `airbnb`, `airbnb/hooks`, `airbnb-typescript`, `plugin:react/recommended`, `plugin:@typescript-eslint/recommended`, and `plugin:prettier/recommended` configurations.

- `overrides`: An array of configurations that are applied to specific files or directories.

- `parser`: Specifies the parser used to parse the code. This project uses the `@typescript-eslint/parser` parser.

- `parserOptions`: An object that specifies the parser options. This project specifies that the latest ECMAScript version is used (`ecmaVersion: 'latest'`), that the source code is in ECMAScript modules (`sourceType: 'module'`), and that the TypeScript project configuration file is located at `./tsconfig.json` (`project: './tsconfig.json'`).

- `plugins`: An array of plugins that are loaded. This project loads the `react`, `@typescript-eslint`, and `prettier` plugins.

- `rules`: An object that specifies the rules to be used. This project does not specify any rules, so all rules from the extended configurations are used.

### Vite Config Options

- `plugins`: An array of Vite plugins.
- `test`: An object with the following properties:
  - `globals`: A boolean that sets whether global variables are enabled for tests. Defaults to `true`.
  - `environment`: A string that sets the test environment. Defaults to `jsdom`.
  - `setupFiles`: An array of strings that specify setup files for tests.
