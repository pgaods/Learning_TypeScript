# Learning TypeScript

TypeScript is a superset of JavaScript, but there's more to it than just type hints. Every valid JavaScript file is valid TypeScript. You can rename a `.js` file to `.ts` and it will work.

Beyond type hints: while type annotations are the most visible difference, TypeScript adds several other features:

- Interfaces and type aliases – define custom types and contracts
- Enums – named constants for sets of values
- Access modifiers – public, private, protected for class members
- Abstract classes – classes that can't be instantiated directly
- Generics – reusable code with type parameters
- Decorators – metadata and function wrapping
- Namespaces – code organization (less common with modules)
- Stricter semantics – catches errors JS allows (like accessing undefined properties)

Key difference in practice: TypeScript is a compiled language (transpiled to JavaScript) that runs through a type checker before compilation. JavaScript runs directly. This means TypeScript catches many errors at development time that would only appear at runtime in JavaScript.

So while you can write TypeScript without type hints (and it would work), you'd miss most of the benefits. TypeScript's value comes from the combination of type safety, advanced language features, and excellent tooling support.

## Textbook

The Textbook is "Learning TypeScript" by Josh Goldberg. The URL for the book is the following:

- <https://www.learningtypescript.com/>

The online version can be found here:

- <https://github.com/SaoodAhmed/Typescript/blob/master/Learning_TypeScript_Josh_Goldberg.pdf>

Errata for the book can be found here:

- <https://www.oreilly.com/catalog/errata.csp?isbn=0636920578000>

## Installation

### Prerequisites

To run JavaScript code, we need to install Node.js first.

1. Install Node.js
   - Download from [nodejs.org](https://nodejs.org)
   - This includes both `node` and `npm`
   - Verify installation:

     ```bash
     node --version
     npm --version
     ```

2. Install TypeScript support (for .jsnb notebooks)

   ```bash
   npm install -g ts-node
   ```

3. Install VS Code extensions (Optional)
   - **JS/TS Notebook Extension** (by Ajay Mall) for `.jsnb` notebooks, or
   - **JavaScript Notebook Extension Pack** (by Gordon Smith) for `.ojsnb` notebooks

Once Node.js is installed and the extensions are in place, you can start using the notebooks.

## Running TypeScript in Notebooks

There are two useful vscode extensions in the market place to run JavaScript and TypeScript files.

### The JS/TS Notebook Extension</span>

The JS/TS Notebook extension designed by Ajay Mall is a good start. Jupyter notebooks will have the file extension `.jsnb`.

### The JavaScript Notebook Extension Pack

The JavaScript Notebook extension pack designed by Gordon Smith is another option. The Jupyter notebooks will have the file extension `.ojsnb`.

### Conventions

We will be using `jsnb` for TypeScript and `.ojsnb` for JavaScript. The most standard way to execute a JavaScript or TypeScript script like how Python executes a `main.py` file is using bash.

To run Javascript code:

```bash
node script.js          # JavaScript
```

To run TypeScript code:

```bash
npx ts-node script.ts   # TypeScript
```