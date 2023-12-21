<div align="center">
  <h1>eslint-plugin-no-bigint-usage</h1>
  <p>Simple eslint plugin to disallow the use of BigInt literals.</p>
</div>

## Installation

```bash
yarn add --dev eslint eslint-plugin-no-bigint-usage
```

**Note:** If you installed ESLint globally then you must also install
`eslint-plugin-no-bigint-usage` globally.

## Usage

Add `no-bigint-usage` to the plugins section of your `.eslintrc` configuration file. You
can omit the `eslint-plugin-` prefix:

```json
{
  "plugins": ["no-bigint-usage"]
}
```

Then configure the rules you want to use under the rules section.

```json
{
  "rules": {
    "no-bigint-usage/no-bigint-literals": "error"
  }
}
```

## Reasons to use this plugin

Older JS engines might display this error if you try to use BigInt literals:

No identifiers allowed directly after numeric literal

This plugin makes sure you don't have BigInt literals in your codebase.
