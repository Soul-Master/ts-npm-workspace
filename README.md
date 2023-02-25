# Example TypeScript monorepo using NPM workspaces

[![Node.js CI](https://github.com/Soul-Master/ts-npm-workspaces/actions/workflows/main.yml/badge.svg)](https://github.com/Soul-Master/ts-npm-workspaces/actions/workflows/main.yml)

An example project that uses NPM workspaces to create a Node.js TypeScript monorepo.

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