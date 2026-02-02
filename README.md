# Git-Cliff Test Project

This project serves as a practical demonstration and testing environment for **git-cliff**, a highly customizable changelog generator.

## Purpose

The main objective is to explore how different [Conventional Commits](https://www.conventionalcommits.org/) and [Semantic Versioning](https://semver.org/) patterns are parsed and categorized into a structured `CHANGELOG.md`.

## Features Demonstrated

- **Breaking Changes**: Using the `!` syntax (e.g., `feat!:`) to trigger major version highlights.
- **Conventional Types**: Testing various prefixes like `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `chore`, and `ci`.
- **Versioning**: Using Git Tags (e.g., `v0.1.0`) to organize the changelog into release sections.
- **Scope Support**: Using parenthesized scopes (e.g., `feat(ui):`) for granular grouping.

## Tools and Skills Used

- **git-cliff**: For generating the [CHANGELOG.md](CHANGELOG.md).
- **flutter-clean-architecture**: The project structure follows Clean Architecture principles (Presentation, Domain, Data layers).
- **git-commit-conventional-cliff-optimized**: A custom skill used to enforce strict commit message formatting optimized for `git-cliff`.

## How to Generate Changelog

To update the changelog after making new commits:

1. **Tag your release** (optional):
   ```bash
   git tag v0.2.0
   ```

2. **Run git-cliff**:
   ```bash
   git-cliff -o CHANGELOG.md
   ```

## Project Structure

```text
lib/
├── core/             # Shared utilities and core logic
└── features/         # Features organized by Clean Architecture layers
    └── calculator/   # Sample feature used for testing
```
