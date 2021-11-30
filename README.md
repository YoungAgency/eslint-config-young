# Young JavaScript Style Guide() {

> This is an opinionated JavaScript guideline for Young devs. Inspired by Airbnb

## Setup

### 1) Install `eslint-config-young` and peer dependencies

```bash
npx install-peerdeps --dev @youngagency/eslint-config-young
```

### 2) Configure ESLint

#### eslint-config-young/hooks

This entry point enables the linting rules for React hooks (requires v16.8+). To use, add `"extends": ["@youngagency/eslint-config-young", "@youngagency/eslint-config-young/hooks"]` to your `.eslintrc`.

#### eslint-config-young/base

This entry point is the base configuration for JavaScript projects (without React). To use, add `"extends": ["@youngagency/eslint-config-young/base"]` to your `.eslintrc`.

#### eslint-config-young/typescript

This entry point enables the linting rules for TypeScript. To use add this to your `.eslintrc`.

```diff
{
  extends: [
    "@youngagency/eslint-config-young",
+   "@youngagency/eslint-config-young/typescript"
  ],
+ parserOptions: {
+   project: './tsconfig.json'
+ }
}
```
