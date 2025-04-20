# Hapnium GitHub Organization

Welcome to **Hapnium's** GitHub Organization!  
This document describes our **repository structure**, **naming conventions**, and **development standards** across all our products and systems.

---

## 📦 Repository Naming Convention

Each **product** we build will generally have up to **three main repositories**:

| Purpose | Repository Name | Example (for `pulse`) |
|:--------|:----------------|:----------------------|
| Backend API (microservices) | `<product>-engine` | `pulse-engine` |
| Public Website (landing/information site) | `<product>-base` | `pulse-base` |
| Mobile App (Flutter/Native app) | `<product>` | `pulse` |
| Web Application (if different from mobile app) | `<product>-webapp` | `pulse-webapp` |

> ℹ️ _`<product>` should be all lowercase, hyphenated if multi-word, e.g., `smartconnect`, `pulse`._

---

### 🏢 Company-Wide Repositories

Some repositories are **shared across all products**. These are general purpose:

| Purpose | Repository Name |
|:--------|:----------------|
| Shared backend libraries and microservices | `engine` |
| Corporate Website (hapnium.com) | `base` |
| Flutter libraries (internal packages) | `flutter` |
| Java libraries and backend tools | `java` |
| Node.js libraries and backend tools | `node` |

> 🛠 **No product name** prefix is used for company-wide repos.

---

## 📚 Folder Structure Recommendations (Per Repository)

Each repository should generally follow this structure:

```
/docs            -> Documentation
/src             -> Source code
/test            -> Tests
/scripts         -> DevOps and automation scripts
/.github         -> GitHub actions, workflows
/README.md       -> Project description
/LICENSE         -> License (if applicable)
```

---

## 🔥 Standards Across All Repos

- **Branch Naming**:  
  `feature/feature-name`, `bugfix/issue-name`, `hotfix/critical-fix`, `release/version`
  
- **Commit Messages**:  
  Follow [Conventional Commits](https://www.conventionalcommits.org/), e.g.,  
  `feat: add login API`, `fix: correct password validation`, `docs: update README`

- **Default Branch**:  
  Always use `main` as the default branch.

- **Licensing**:  
  Each repository must include a `LICENSE` file (default is private license unless stated otherwise).

- **Documentation**:  
  Every repository must include a `README.md` describing:
  - Purpose
  - Installation Instructions
  - Contribution Guide (if open internally)
  - Build and Deployment Instructions

- **Pull Requests**:  
  - PRs must be linked to issues where applicable.
  - PRs must have at least one code reviewer before merging (even self-reviewed if solo).
  
- **Security**:  
  - Secrets must never be committed into repositories.
  - Use environment variables and GitHub Secrets for pipelines.
  - MFA should be enabled for critical user accounts.

---

## 🚀 Example for a Product: **Pulse**

| Purpose | Repo Name | Notes |
|:--------|:----------|:------|
| Backend Server | `pulse-engine` | Spring Boot backend APIs |
| Public Website | `pulse-base` | Landing page built with Next.js |
| Mobile App | `pulse` | Flutter mobile app |
| Web App (Separate) | `pulse-webapp` | Web dashboard |

---

## ✨ About Hapnium

At **Hapnium**, we are passionate about building scalable, secure, and elegant software solutions for the modern world.  
We maintain high standards across all our products and development practices.

- 🌐 Website: [hapnium.com](https://hapnium.com) _(coming soon)_
- 📧 Contact: [info@hapnium.com](mailto:info@hapnium.com)
- 📍 Based in: UTC +01:00

---

# Let's build the future. 🚀
