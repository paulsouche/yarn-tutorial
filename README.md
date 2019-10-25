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
