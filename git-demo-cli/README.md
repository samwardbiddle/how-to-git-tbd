oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![GitHub license](https://img.shields.io/github/license/oclif/hello-world)](https://github.com/oclif/hello-world/blob/main/LICENSE)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g git-demo-cli
$ git-demo-cli COMMAND
running command...
$ git-demo-cli (--version)
git-demo-cli/0.0.0 darwin-x64 node-v20.5.1
$ git-demo-cli --help [COMMAND]
USAGE
  $ git-demo-cli COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`git-demo-cli hello PERSON`](#git-demo-cli-hello-person)
* [`git-demo-cli hello world`](#git-demo-cli-hello-world)
* [`git-demo-cli help [COMMANDS]`](#git-demo-cli-help-commands)
* [`git-demo-cli plugins`](#git-demo-cli-plugins)
* [`git-demo-cli plugins:install PLUGIN...`](#git-demo-cli-pluginsinstall-plugin)
* [`git-demo-cli plugins:inspect PLUGIN...`](#git-demo-cli-pluginsinspect-plugin)
* [`git-demo-cli plugins:install PLUGIN...`](#git-demo-cli-pluginsinstall-plugin-1)
* [`git-demo-cli plugins:link PLUGIN`](#git-demo-cli-pluginslink-plugin)
* [`git-demo-cli plugins:uninstall PLUGIN...`](#git-demo-cli-pluginsuninstall-plugin)
* [`git-demo-cli plugins:uninstall PLUGIN...`](#git-demo-cli-pluginsuninstall-plugin-1)
* [`git-demo-cli plugins:uninstall PLUGIN...`](#git-demo-cli-pluginsuninstall-plugin-2)
* [`git-demo-cli plugins update`](#git-demo-cli-plugins-update)

## `git-demo-cli hello PERSON`

Say hello

```
USAGE
  $ git-demo-cli hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [src/commands/hello/index.ts](https://github.com/swbxyz/git-demo-cli/blob/v0.0.0/src/commands/hello/index.ts)_

## `git-demo-cli hello world`

Say hello world

```
USAGE
  $ git-demo-cli hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ git-demo-cli hello world
  hello world! (./src/commands/hello/world.ts)
```

_See code: [src/commands/hello/world.ts](https://github.com/swbxyz/git-demo-cli/blob/v0.0.0/src/commands/hello/world.ts)_

## `git-demo-cli help [COMMANDS]`

Display help for git-demo-cli.

```
USAGE
  $ git-demo-cli help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for git-demo-cli.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.20/src/commands/help.ts)_

## `git-demo-cli plugins`

List installed plugins.

```
USAGE
  $ git-demo-cli plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ git-demo-cli plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.9.1/src/commands/plugins/index.ts)_

## `git-demo-cli plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ git-demo-cli plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ git-demo-cli plugins add

EXAMPLES
  $ git-demo-cli plugins:install myplugin 

  $ git-demo-cli plugins:install https://github.com/someuser/someplugin

  $ git-demo-cli plugins:install someuser/someplugin
```

## `git-demo-cli plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ git-demo-cli plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ git-demo-cli plugins:inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.9.1/src/commands/plugins/inspect.ts)_

## `git-demo-cli plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ git-demo-cli plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ git-demo-cli plugins add

EXAMPLES
  $ git-demo-cli plugins:install myplugin 

  $ git-demo-cli plugins:install https://github.com/someuser/someplugin

  $ git-demo-cli plugins:install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.9.1/src/commands/plugins/install.ts)_

## `git-demo-cli plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ git-demo-cli plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help      Show CLI help.
  -v, --verbose
  --[no-]install  Install dependencies after linking the plugin.

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ git-demo-cli plugins:link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.9.1/src/commands/plugins/link.ts)_

## `git-demo-cli plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ git-demo-cli plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ git-demo-cli plugins unlink
  $ git-demo-cli plugins remove
```

## `git-demo-cli plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ git-demo-cli plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ git-demo-cli plugins unlink
  $ git-demo-cli plugins remove
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.9.1/src/commands/plugins/uninstall.ts)_

## `git-demo-cli plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ git-demo-cli plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ git-demo-cli plugins unlink
  $ git-demo-cli plugins remove
```

## `git-demo-cli plugins update`

Update installed plugins.

```
USAGE
  $ git-demo-cli plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.9.1/src/commands/plugins/update.ts)_
<!-- commandsstop -->
