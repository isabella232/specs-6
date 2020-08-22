---

⚠ This repository is not actively used any more, please check out the [Prisma Documentation](https://docs.prisma.io) for updated information on Prisma. ⚠

---

# Prisma Framework Specifications 

This repository contains specifications for Prisma Framework:

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [About this repository](#about-this-repository)
- [Specifications](#specifications)
  - [User facing parts](#user-facing-parts)
  - [Internal parts](#internal-parts)
  - [Organisation](#organisation)
    - [Process](#process)
    - [Meta](#meta)
  - [Style Guide](#style-guide)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## About this repository

This repository is designed to help different groups of people:

- Prisma Product: Specify and work on new and existing functionality 🛫
- Prisma Engineering: Collaborate with Product and use specs as base for implementation work 👩‍💻
- Prisma Community and Users: Follow and understand Prisma Framework development 👽

Besides the [specifications](#specifications) linked below, most of the work here happens in [the repo issues](https://github.com/prisma/specs/issues) and [pull requests](https://github.com/prisma/specs/pulls).

## Specifications

### User facing parts

Prisma Framework consists of several tools:

- [Prisma Schema Language](schema) (PSL)
- Tools
  - [Prisma CLI](cli) - setup and introspection
  - Prisma Client - data access
    - [Prisma Client JS](prisma-client-js)
    - [Prisma Client Go](prisma-client-go)
  - [VSCode Prisma](vscode-extension) - PSL formatting and linting
  - [Prisma Migrate](migrate) - migrate databases
  - [Prisma Studio](studio) - GUI

### Internal parts

It also has several internal parts:

- [SDK](sdk)
  - [JS SDK](sdk-js)
    - [Generators](sdk-js/generators)
    - [Engine Runtime](sdk-js/engine-runtime)
- [Binaries](binaries)
- [Errors](errors)

### Organisation

We don't only spec the software itself, but also how we work on it and on these sepcs:

#### Process

- [GitHub labels](process/labels.md)
- [Issue Triage](process/issue-triage.md)
- [Repositories](process/repositories.md)

#### Meta

- [Specs](meta/specs.md)
- [Table of Contents](meta/table-of-contents.md)

### Style Guide

Please run `prettier` on every `.md` file before committing with the following configuration (ideally via this [VSC extension](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)):

```json
  "prettier.singleQuote": true,
  "prettier.trailingComma": "all",
  "prettier.semi": false,
```
