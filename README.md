# Oracle Commerce Cloud CLI

[![GitHub contributors](https://img.shields.io/github/contributors/eduardokeneeth/oracle-commerce-cli?style=flat-square)](https://github.com/eduardokeneeth/oracle-commerce-cli/graphs/contributors)
[![npm](https://img.shields.io/npm/v/oracle-commerce-cli?label=last%20version&style=flat-square)](https://www.npmjs.com/package/oracle-commerce-cli)
[![npm](https://img.shields.io/npm/dt/oracle-commerce-cli?style=flat-square)](https://www.npmjs.com/package/oracle-commerce-cli)

A simple CLI to help with your daily OCC development.

## Prerequisites
- Your project shoud follow [this structure](https://github.com/eduardokeneeth/oracle-commerce-project-example).

# Installation
```sh
npm install -g oracle-commerce-cli
```

# Getting Started

After installing the CLI and make sure your project is following the prerequisites you need to start your project using `occ --start`. At this point you will inform your current environment and pass the URL + AppKey.

```sh
$ occ --start
? Select an environment: TEST
? Admin URL: <URL>
? AppKey: <KEY>
Your project is ready!
```

After this you can use everything on this CLI. 

**Note:** You only need to do this once, after that if you need to update, change or configure an environment, please use the Environment Manager (`occ --env <operation>`).

# Options

The following table describes the options you can use with `occ`.

|Option|Description|
|:---|:---|
| `-h, --help` | Provides usage information for the CLI |
| `-V, --version` | Provides the CLI's version |
| `-s, --start` | Starts the project setup |
| `-d, --dev` | Starts Watcher + Browsersync. <br><br> **Note:** [Click here](https://github.com/eduardokeneeth/oracle-commerce-project-example#browsersync) to see how configure Browsersync. |
| `-c, --create <type>` | Creates widget or element. <br><br> **Options:** `widget`, `element`. |
| `-r, --refresh <path>` | Refreshes content from the Commerce instance within the specified directory. |
| `-p, --putAll <path>` | Sends everything from the specified directory. |
| `-e, --env <operation>` | Starts the Environment Manager. <br><br> **Options:** `current`, `config`, `change`. |
| `-t, --transfer <path>` | Transfers things between current and selected environment. |
| `-g, --grab <path>` | Starts grabbing everything from current environment. |

# License
Oracle Commerce CLI is [MIT licensed](https://github.com/eduardokeneeth/oracle-commerce-cli/blob/master/LICENSE).