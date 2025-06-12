# Conventional Commit Cheatsheet

A comprehensive guide to standardize your commit messages using the Conventional Commits specification. This repository provides developers with a structured reference for implementing the Conventional Commits standard in their Git workflow, including commit types, formatting rules, and best practices.

## 📚 Overview

Conventional Commits provide a lightweight convention on top of commit messages, offering a simple set of rules for creating an explicit commit history. This standardized format makes your project history clear, consistent, and machine-readable, enabling:

- Automatic versioning and release notes
- Clear communication of changes to teammates
- Easier maintenance and collaboration on projects
- Better organization of git history

This cheatsheet serves as a quick reference guide for developers looking to implement Conventional Commits in their workflow.

## 🚀 Usage

### Basic Commit Structure

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Quick Start

1. **Make changes** to your codebase
2. **Stage your changes**:
   ```bash
   git add <files>   # Specific files
   git add .         # All changes
   ```
3. **Create a conventional commit**:
   ```bash
   git commit -m "feat(auth): add login with Google feature"
   ```
4. **Push your changes**:
   ```bash
   git push origin <branch-name>
   ```

## ✨ Features

Conventional Commits provide several key benefits:

- **Automatic Versioning**: Enables semantic versioning based on commit types
- **Improved Readability**: Makes commit history clear and understandable
- **Automated Tools**: Enables automating changelogs and release notes
- **Better Collaboration**: Helps teams understand changes at a glance
- **Structured History**: Creates a well-organized project history
- **Integration with CI/CD**: Facilitates automated testing and deployment
- **Simplified Code Reviews**: Makes code reviews more efficient

## 📋 Commit Types & Descriptions

### Primary Types

| Type       | Description                                               | Example                                        |
| ---------- | --------------------------------------------------------- | ---------------------------------------------- |
| `feat`     | A new feature                                             | `feat(auth): add login button`                 |
| `fix`      | A bug fix                                                 | `fix(button): resolve click event issue`       |
| `docs`     | Documentation changes                                     | `docs: update API usage examples`              |
| `style`    | Code style changes (formatting, missing semicolons, etc.) | `style: apply consistent indentation`          |
| `refactor` | Code changes that neither fix bugs nor add features       | `refactor: simplify authentication logic`      |
| `test`     | Adding or correcting tests                                | `test(api): add unit tests for user endpoints` |
| `chore`    | Maintenance tasks like dependencies or build changes      | `chore: update npm packages`                   |

### Secondary Types

| Type     | Description                                        | Example                                     |
| -------- | -------------------------------------------------- | ------------------------------------------- |
| `build`  | Changes affecting the build system or dependencies | `build(deps): upgrade webpack to v5`        |
| `ci`     | Changes to CI configuration files and scripts      | `ci(github): update action workflow`        |
| `perf`   | Performance improvements                           | `perf(images): optimize image loading`      |
| `revert` | Reverts a previous commit                          | `revert: feat(auth): add login with Google` |
| `env`    | Environment setup or configuration changes         | `env(docker): update staging configuration` |
| `sec`    | Security-related changes                           | `sec(auth): implement rate limiting`        |
| `config` | Configuration file updates                         | `config: update eslint rules`               |
| `api`    | API contract or integration updates                | `api(user): add profile endpoint`           |
| `deps`   | Dependency-specific updates                        | `deps: upgrade axios to v1.0.0`             |
| `design` | UI/UX improvements                                 | `design(button): enhance hover effects`     |

### Adding Scope (Optional)

The scope provides context about what part of the codebase is affected:

```bash
git commit -m "feat(authentication): add password reset flow"
```

### Breaking Changes

For breaking changes, add `!` after the type/scope:

```bash
git commit -m "feat(api)!: change response format of user endpoints"
```

Or include `BREAKING CHANGE:` in the commit body:

```bash
git commit -m "feat(api): change response format of user endpoints

BREAKING CHANGE: The response format has been modified to follow JSON:API specification"
```

## 📖 Additional Resources

- [Official Conventional Commits Specification](https://www.conventionalcommits.org)
- [Semantic Versioning](https://semver.org/)
- [Angular Commit Message Guidelines](https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit)

---

<div align="center">
  <p>Made with ❤️ for better commit histories</p>
  <p><img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License"></p>
</div>
