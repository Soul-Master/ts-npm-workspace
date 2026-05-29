# TypeScript NPM Workspace

[![CI Status](https://github.com/Soul-Master/ts-npm-workspaces/actions/workflows/main.yml/badge.svg)](https://github.com/Soul-Master/ts-npm-workspaces/actions/workflows/main.yml)
![Node](https://img.shields.io/badge/dynamic/json?label=node&query=$.engines.node&url=https://raw.githubusercontent.com/Soul-Master/ts-npm-workspace/main/package.json)
![ES target](https://img.shields.io/badge/dynamic/json?label=ES&query=$.compilerOptions.target&url=https://raw.githubusercontent.com/Soul-Master/ts-npm-workspace/main/tsconfig.base.json)

A minimal TypeScript monorepo showing TypeScript composite projects/NPM packages for Node.js, browser and shared environment.

```mermaid
flowchart TD
  core["@demo/core<br/>Shared package"]
  cli["@demo/cli<br/>Node.js-based package"]
  web["@demo/web<br/>Browser-based package"]

  cli --> core
  web --> core
```

## Getting started

```
npm start
```

## Run it

**CLI module**

```
npm start -w @demo/cli
```

**Web module**

```
npm start -w @demo/web
```

**All possible packages**

```
npm start --workspaces --if-present
```
