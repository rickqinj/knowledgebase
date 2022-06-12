# TypeScript Learning Note

### Questions need to be solved

This section is only used for me(the author) to taking notes on questions that I come across during I learn TypeScript.

- Try out several kinds of inheritance/implementation patterns with:
  - Class extends class; How to do it? What's the practical usecase, if any;  
  - Class implement interface;
  - Interface extends interface;
  - Interface extends more than one interfaces;
  - Interface extends from class;
  - Experiment: Can we do multiple inheritance in TypeScript? If so, how to do and when is it applicable?
  - Experiment: Interface extends from a class. And what's the use of the interface?
- Concept: 
  - What is a module in TypeScript?
    - 
  - What do we do commonly with modules in TypeScript project?
  - How can we access to or customize our own modules?

## Content

- [Initialize a TypeScript project](#initialize-a-typescript-project)
- [Module and its related knowledge](#module-and-its-related-knowledge)
  - [What is a module in TypeScript](#what-is-a-module-in-typescript)
  - 
- 

## Initialize a TypeScript project

We can follow the steps listed below to initialize a TypeScript project.

1. Go to the project folder, for example, `D:\mytsprj`.

```shell
> cd d:\mytsprj
d:\mytsprj\>
```

2. In the project folder, execute the following command.

```shell
d:\mytsprj\> npx tsc --init

Created a new tsconfig.json with:

  target: es2016
  module: commonjs
  strict: true
  esModuleInterop: true
  skipLibCheck: true
  forceConsistentCasingInFileNames: true


You can learn more at https://aka.ms/tsconfig
d:\mytsprj\>
```

## Module and its related knowledge

### What is a module in TypeScript

A module in TypeScript usually comes as a file(*.ts) which contains classes, interfaces, variables, values and functions(methods).

