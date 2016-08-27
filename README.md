# pleaserc

Linting configuration for ESLint and Stylelint.

### About

These are the linting rules that I use. They're inspired by coding styles that I
observe as being common, such as always using braces and requiring semicolons
in JavaScript.

#### The JavaScript rules

The rules are less opinionated on a few issues. For instance,

- you can still use `var` (rather than `let` or `const`)
- it won't explode if you use `const` on unmodified variables
- trailing commas can be there, or they can be omitted.
- arrow functions with a single argument can have parentheses or not

On other issues, things are more strict. For instance, "fixme" and "todo"
comments will cause the linting to fail. Clean-up tasks belong in an issue
tracker, I think.

If you're looking for linting rules that try to strike a middle ground between
being opinionated without being too overbearing, then these might be a good
starting off point.

### Usage

Install via npm.

```sh
npm install pleaserc
```

Then, in your linting config file,

```
{
  "extends": "./node_modules/pleaserc/.eslintrc",
  "rules": {
    // Override some rules here
  }
}
```
