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
