---
sidebar_position: 1
---

# Intro

Let's discover **Chainify in less than 5 minutes**.

## Getting Started

Chainify exists to help developers build chain-agnostic applications. It's designed to run in any environment that can execute JavaScript (think websites, node scripts, etc.). While simple enough to use in a hackathon project, it's also robust enough to power production applications.

## Installation

The easiest way to consume Chainify is via npm. 

```bash
yarn add @chainify/<package_name>
```

or

```bash
npm install @chainify/<package_name>
```

:::note
You can see all available packages **[here](./packages/modules.md)**. 
::: 


## Local development

[The repository](https://github.com/liquality/chainify) uses [yarn workspaces](https://yarnpkg.com/features/workspaces) for fast, reliable, and secure dependency management.

The build system is using [Turborepo](https://turborepo.org/)

#### Build all packages
```bash
yarn build
```
#### Run all tests
```bash 
yarn test
```