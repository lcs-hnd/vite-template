# vite-template

> Vite development template. Includes opinionated linting, QOL tools.

---

## Dependencies

- **prettier**: Enforces consistent code formatting.

- **eslint** + **@eslint/js**: Lints JavaScript for common mistakes and enforces best practices.

- **eslint-config-prettier**: Turns off ESLint rules that would conflict with Prettier.

- **stylelint** + **sylelint-config-standard**: CSS linting based on standard conventions, improving maintainability of styles.

- **stylelint-order**: Enforces logical property grouping and ordering for cleaner stylesheets.

- **concurrently**: Runs multiple linters in watch mode at once with clean, organized output.

## Config Files

**.eslint.config.mjs**

> Uses the flat ESLint config with @eslint/js as the base. Adds Prettier compatibility and a small set of project-agnostic quality rules (e.g., no-var, prefer-const).

**.stylelintrc.json**

> Extends stylelint-config-standard with custom property groups and ordering logic. Prioritizes CSS readability and visual hierarchy by grouping properties like layout, box model, and typography.

**.prettierrc**

> A concise Prettier setup enforcing single quotes, semi-colons, and a consistent print width (80) for balanced readability and diff clarity.

**.prettierignore**

> Excludes folders like dist, node_modules, and build artifacts from formatting to speed up Prettier runs and avoid unnecessary churn.

## Default Scripts

- `dev`: Start Vite development server.

- `build`: Build the app for production.

- `preview`: Preview the production build locally.

- `lint:js`: Build the app for production.

- `lint:css`: Build the app for production.

- `lint`: Run both JS and CSS linters.

- `format`: Format all files with Prettier.

- `format:check`: Check formatting without applying changes.

- `fix:all`: Auto-fix lint and formatting issues.

- `watch`: Watching JS and CSS for linting and auto-fixing in real time.
