# env-sync

**env-sync** is a command-line tool designed to simplify the management of environment (`.env`) files across multiple projects and environments. It helps you keep your `.env` files in sync with your `.env.example` or other configuration templates, making sure you're always up-to-date with the required environment variables.

## Key Features:

- Compare `.env` files with `.env.example` to identify missing or extra variables.
- Automatically update `.env.example` with missing keys from `.env`.
- Support for passing custom environment files via CLI.
- Compare multiple `.env` files and identify discrepancies.
- Optionally preserve or remove comments during comparison.
- Regular expression support for comparing multiple file names.
- Easy integration with Git hooks (e.g., Husky) for pre-commit or pre-push checks.

## Why use env-sync?

Working in teams or managing multiple projects with different environments (`.env`, `.env.prod`, `.env.local`, etc.) can be a challenge. **env-sync** automates the comparison and synchronization of your environment files, helping you maintain consistency across all environments.

## Todo

- Compare and create / update the `.env.example` based on `.env` file.
  - There should be a command line option to pass different file name either than going with standard `.env` or `.env.example`
  - Should be able to pass cli option to keep comments in `.env` file or not while generating a new `.env.example` or some other similar file based on `.env`
- Compare multiple `.env` file and list down the property missing or extra in any of them
  - Should be able to pass the source file
  - Should be able to pass the multiple file names to compare / regex for file names
  - Should be able to compare only key or both key-value pair
