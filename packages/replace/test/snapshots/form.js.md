# Snapshot report for `test/form.js`

The actual snapshot is saved in `form.js.snap`.

Generated by [AVA](https://avajs.dev).

## assignment: doesn't replace lvalue in assignment

> Snapshot 1

    'process.env.DEBUG = \'test\';'

## delimiters: observes delimiters

> Snapshot 1

    `console.log(\`␊
      replaced␊
      <% original%>␊
      <%original %>␊
    \`);`

## match-variables: matches most specific variables

> Snapshot 1

    'console.log(\'beta version 1.0.0\');'

## observe-plugin-options: does not replace plugin options

> Snapshot 1

    `console.log(\`␊
      replaced␊
      delimiters␊
      sourcemap␊
      sourceMap␊
      include␊
      exclude␊
      preventAssignment␊
      values␊
    \`);`

## process-check: Handles process type guards in replacements

> Snapshot 1

    `if ("object" !== 'undefined' && "object" === "object" && "production" === 'production') {␊
      console.log('production');␊
    }`

## replace-nothing: replaces nothing

> Snapshot 1

    `console.log('as-it'); // eslint-disable-line␊
    console.log(typeof window.document); // eslint-disable-line`

## replace-strings: replaces strings

> Snapshot 1

    `console.log(42); // eslint-disable-line␊
    console.log("object");`

## replacement-function: allows replacement to be a function

> Snapshot 1

    'export default "input.js";'

## special-characters: supports special characters

> Snapshot 1

    `const one = 1; // eslint-disable-line␊
    ␊
    console.log(one);`

## special-delimiters: allows delimiters with special characters

> Snapshot 1

    `console.log(\`␊
      replaced␊
      (replaced)␊
      specially␊
      especial␊
      replaced.doSomething()␊
    \`);`

## ternary-operator: replaces value inside ternary operators

> Snapshot 1

    `/* eslint-disable */␊
    first ? second : third;␊
    console.log(first, second, third);`

## typescript-declare: doesn't replace lvalue in typescript declare

> Snapshot 1

    `declare const NAME: string␊
    console.log(replaced)`
