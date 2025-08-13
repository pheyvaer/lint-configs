# Lint configs for JavaScript and Markdown

- JavaScript
  - Tool: [ESLint](https://eslint.org/)
  - Config file: `eslint.config.js`
- Markdown
  - Tool: [markdownlint-cli2](https://github.com/DavidAnson/markdownlint-cli2)
  - Config file: `.markdownlint-cli2.cjs`

You find scripts to run these tools in `package.json`:

```json
{
  "lint:js": "eslint . --ext js --report-unused-disable-directives --max-warnings 0",
  "lint:js:fix": "eslint . --ext js --report-unused-disable-directives --max-warnings 0 --fix",
  "lint:markdown": "markdownlint-cli2",
  "lint:markdown:fix": "markdownlint-cli2 --fix"
}
```
