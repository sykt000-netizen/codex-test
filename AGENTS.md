# Repository Guidelines

## Project Structure & Module Organization
- Root contains `README.md` and this contributor guide. No source modules exist yet.
- When adding code, place runtime code under `src/` and tests under `tests/` to keep paths predictable (e.g., `src/index.js`, `tests/index.test.js`).
- Keep assets (images, fixtures) under `assets/` or `tests/fixtures/` so tooling can ignore them when needed.

## Build, Test, and Development Commands
- No build or test scripts are defined in this repository yet.
- If you introduce tooling, add standard commands and document them here, for example:
  - `npm run build` to compile source to `dist/`.
  - `npm test` to run the test suite.
  - `npm run lint` to enforce formatting and style.

## Coding Style & Naming Conventions
- Use consistent, readable formatting; prefer 2-space indentation for new JavaScript/TypeScript files unless the project establishes another style.
- Name files and directories with lowercase, hyphenated names (e.g., `data-loader.js`).
- Keep public entry points small and place implementation details in `src/` submodules.

## Testing Guidelines
- No testing framework is configured.
- If you add tests, choose a single runner (e.g., Jest, Vitest) and keep test filenames adjacent or in `tests/` with a `.test.*` suffix (e.g., `user.test.ts`).
- Add at least one test for new features and document how to run them.

## Commit & Pull Request Guidelines
- Git history only includes `Initial commit`, so no established convention exists.
- Use short, imperative commit messages (e.g., "Add parser for config files").
- PRs should include a brief description, testing notes, and any relevant screenshots or logs for visible changes.

## Security & Configuration Tips
- Do not commit secrets or local configuration. Use `.env` files and add them to `.gitignore` if needed.
- Document required environment variables in `README.md` and keep defaults safe for local development.
