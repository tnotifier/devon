<div align="center">
    <a href="https://www.npmjs.com/package/@casthub/devon" target="_blank">
        <img src="https://img.shields.io/npm/v/@casthub/devon?style=flat-square" alt="NPM" />
    </a>
    <a href="https://discord.gg/XMrHXtN" target="_blank">
        <img src="https://img.shields.io/discord/123906549860139008?color=7289DA&label=discord&logo=discord&logoColor=FFFFFF&style=flat-square" alt="Discord" />
    </a>
    <img src="https://img.shields.io/npm/l/@casthub/devon?style=flat-square" alt="Apache-2.0" />
    <h3>Docker-based Monorepo Local Development CLI</h3>
</div>

> **This is a work-in-progress!**

`@casthub/devon` is a node-based CLI tool aiming to bridge the gap between production and local development for monorepos.

- Configure multi-command Scripts for common development workflows
- Generate `.env` files automatically based on the target environment
- Run production-grade images locally without having to touch `docker` commands
- Bootstrap existing Monorepos with intelligent initialization
- TypeScript definitions/configs

## Installation

This package is available via NPM:

```bash
yarn global add @casthub/devon

# or

npm install -g @casthub/devon
```

**You also need to have Docker installed on your local machine.** It can be downloaded via [docker.com](https://www.docker.com/products/docker-desktop).

## Usage

`devon help` lists all available commands and usage. Some useful commands to get you started are:

- `devon init` - Initialize `devon` in the current working directory. This should be the root of your monorepo.
- `devon switch` - Switch which services/apps you are currently working on.
- `devon run <name...>` - Run the given Script(s).
- `devon exec <name> <command...>` - Run a command inside the container for a service.

## To-do

- Add mkcert support & automation
- Add test suite
