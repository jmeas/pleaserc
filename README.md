# pleaserc

Linting configuration for ESLint.

### About

These are the ESLint rules that I use. They're inspired by coding styles that I
observe as being common, such as always using braces and requiring semicolons.

They're also lenient on a few issues, such as:

- never using `var`
- preferring `const` for unmodified variables
- trailing commas
- having an opinion on parentheses for arrow functions with a single argument

On other issues, the rules are more strict. For instance, "fixme" and "todo"
comments will cause the linting to fail. Clean-up tasks belong in an issue
tracker, I think.

If you're looking for linting rules that try to strike a middle ground between
being opinionated without being too overbearing, then you might want to try
these out.

### Usage

Install via npm.

```sh
npm install pleaserc
```

Then, in your ESLint file,

```
{
  "extends": "./node_modules/pleaserc/.eslintrc",
  "rules": {
    // Override some rules here
  }
}
```
