# Yarn tutorial

This repository is a tutorial about `yarn`. Feel free to checkout the step branches.

## Bootstrap a project

`yarn init`

## Add dependencies

`yarn add colors`

`yarn add -D typescript ts-node`

## Recover dependencies

`git clean -fdx`

`yarn` or `yarn install`

`yarn --frozen-lockfile` or `yarn install --frozen-lockfile` install dependencies following `yarn.lock` and **fails** if any compatibility detected with `package.json`

`yarn --ignore-scripts` or `yarn install --ignore-scripts` install dependencies without executing `postinstall scripts`

`yarn --ignore-engines` or `yarn install --ignore-engines` install dependencies and ignore `engines` versions

## Helpers command

`yarn audit` outputs potential security issues with your dependencies

`yarn check` checks the current version of your dependencies against the `package.json`

`yarn info <package>` outputs the `npm info <package>` "json" format

`yarn list --depth=<depth>` outputs the `npm list --depth=<depth>`

`yarn licenses list` outputs all the licences of the dependencies

`yarn versions` outputs usefull versions (node, yarn, v8 ...)

`yarn why <package>` outputs dependency tree explaining why you have this package in your `node_modules`

## Manage your dependencies

`yarn outdated` outputs outdated dependencies

`yarn upgrade` or `yarn upgrade <package>` update the dependency following package.json

`yarn upgrade-interactive` updates a list of dependencies

## Run scripts

`yarn start` executes the start script `yarn run start` also

`yarn ts-node` execcutes the ts-node command

`yarn bin` outputs the resolved `.bin folder`

`yarn node` runs node command with the same version than yarn

## Administrate

### Admin commands

`yarn global [add|remove|list|bin]` administrate global packages

`yarn cache [list|clean|dir]` administrate cache

`yarn config` same than `npm config`

### Registry commands

`yarn login` logs in the yarn registry `--registry` to specify an other registry

`yarn logout` logs out of the registry

`yarn publish` publish the package

`yarn team`, `yarn owner`, `yarn tag` manage the registry users & versions

### Package commands

`yarn create` fetch a `create-*` boilerplate and inits a project

`yarn pack` create the package tarball locally (very usefull to see what is going to be published)

`yarn link` create a symbolic link between the package and the node_modules of the project that consumes it

`yarn unlink` destroy the symbolic link

`yarn version` change the package version

`yarn autoclean` clean dependencies

`yarn generate-lock-entry` generates the lock hash for the package

`yarn import` generates `yarn.lock` from `package-lock.json`
