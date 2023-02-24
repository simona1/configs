# TypeScript



## Installation

The packages below are required:

```
yarn add --dev --exact typescript ts-node ts-loader
```

To initialize a TypeScript project, run this command:

```
yarn tsc --init
```
This will create a `tsconfig.json` file in the root of your project directory. The `tsc` part of the command refers to the TypeScript compiler (listed above as a prerequisite).


## Configuration

Whereas the defaults included in the auto-generated `tsconfig.json` file are reasonable, there are a few recommended changes:

* Set `"jsx": "react"` 
  This indicates to the TypeScript compiler that your code is using JSX syntax. Recommended for React applications.

* Uncomment the `"noEmit": "true"` option
  This tells the TypeScript compiler to do just type-checks, without generating any output files. This option can be useful when TypeScript is used as a dev tool to catch type-related errors before deploying the code.



## Additional

For an npm/yarn script add the script below to `package.json`. This will typecheck the files in the directory indicated by the path `-p ` flag. 

```json
{
  "scripts": {
    "typecheck": "tsc -p REPLACE-WITH-YOUR-DIRECTORY-TO-BE-TYPECHECKED"
  }
}
```

In addition to packages used for a project, you may need to install type definitions for these packages. 
The `@types` notation is used to differentiate type definition packages from regular packages. For example, the package react provides the React library, while the package `@types/react` provides the type definitions for the React library. When a package is installed with type definitions, it is automatically included in your project's type checking process.

For example, for a project that uses `node`, `express`, `react`, and `jest` install their type definitions as dev dependencies:

```
yarn add --save-dev --exact \
  @types/express \
  @types/jest \
  @types/node \
  @types/react \
  @types/react-dom
```