# CLAIR-LAB-TECHNION Coding Standards

This document outlines the basic rules we have agreed upon for all coding projects under the CLAIR-LAB-TECHNION organization.

## Repository Management
- All repositories must be hosted under [CLAIR-LAB-TECHNION GitHub organization](https://github.com/CLAIR-LAB-TECHNION).

## Code Quality and Testing
- Every function added to the codebase must have an accompanying test suite.
- Each repository must include a GitHub Action that automatically checks that all tests pass before allowing the creation of a pull request.

## Code Organization
- Environment and algorithmic development must be kept in separate modules with no co-dependencies.
  - For example, files that define environments must not import libraries focused on algorithms.

## Installation Management
- Installation dependencies must be separated between environment and algorithmic components.
- A dedicated `[test]` section should be created in the installation file (e.g., `setup.cfg`) for installing testing dependencies.
  - For example, in [energy-net setup.cfg](https://github.com/CLAIR-LAB-TECHNION/energy-net/blob/main/setup.cfg), we define a `[test]` section that installs `sb3` for testing the custom Gym environment.

---

Please adhere to these standards to ensure clarity, maintainability, and reproducibility across all our projects.
