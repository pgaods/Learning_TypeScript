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

## Running TypeScript in Notebooks

There are two useful vscode extensions in the market place to run JavaScript and TypeScript files.

### The JS/TS Notebook Extension</span>

The JS/TS Notebook extension designed by Ajay Mall is a good start. Jupyter notebooks will have the file extension `.jsnb`.

### The JavaScript Notebook Extension Pack

The JavaScript Notebook extension pack designed by Gordon Smith is another option. The Jupyter notebooks will have the file extension `.ojsnb`.
