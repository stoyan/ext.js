# .ext.js

Common JavaScript file extensions in the wild

## .js

This is a generic JavaScript file. May run in the browser like:

```html
  <script src="name.js"></script>
```  
  
But it may not run successfully, in case it uses syntax that is not yet available in browsers and it needs a build (transpilation) step using something like [Babel](https://babeljs.io/).
  
Potentially may run in [Node](https://nodejs.org/), like:
```
  $ node name.js
```
## .mjs

This is a JavaScript _module_. Browser usage:

```html
  <script type="module" src="name.mjs"></script>
```

It can `export` and also `import` other modules. [More](http://exploringjs.com/es6/ch_modules.html#sec_basics-of-es6-modules).

## .json

A JSON (JavaScript Object Notation) file. Not JavaScript code, but a piece of data. Commonly used for project configuration under the name `package.json`.

## .ts

TypeScript file. [TypeScript](https://www.typescriptlang.org/) is JavaScript + static variable types. You don't load them in the browser, a build step is necessary.

## .d.ts

A custom type definitions for TypeScript. This is not code meant to be executed, but rather to help define a type to be used in a `.ts` file.

## .bundle.js

A production-ready build usuially including several .js _source_ files _bundled_ into one. If there's bleeding-edge JS syntax in the source files, these are transpiled into syntax that the browsers understand, e.g. ECMAScript 3. Comonnly minified too.

## .min.js

A minified bundle of JavaScript code meant for production web sites.

## .jsx

Superset of JavaScript that let's us define markup in the code. Originated by [React](https://reactjs.org/).

```js
  const name = 'Josh Perez';
  const element = <h1>Hello, {name}</h1>;
```

[source](https://reactjs.org/docs/introducing-jsx.html)

## .tsx

TypeScript version of JSX.
