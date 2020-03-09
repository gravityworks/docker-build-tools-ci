# Docker Build Tools CI

This is the source Dockerfile for the [gravityworks/docker-build-tools-ci](https://hub.docker.com/repository/docker/kurttrowbridge/docker-build-tools-ci/) Docker image, based off of [pantheon-public/build-tools-ci](https://quay.io/repository/pantheon-public/build-tools-ci).

## Image Contents

- [CircleCI PHP 7.3, Node, Headless browser Docker base image](https://hub.docker.com/r/circleci/php)
- [Terminus](https://github.com/pantheon-systems/terminus)
- Terminus plugins
  - [Terminus Build Tools Plugin](https://github.com/pantheon-systems/terminus-build-tools-plugin)
  - [Terminus Secrets Plugin](https://github.com/pantheon-systems/terminus-secrets-plugin)
  - [Terminus Rsync Plugin](https://github.com/pantheon-systems/terminus-rsync-plugin)
  - [Terminus Quicksilver Plugin](https://github.com/pantheon-systems/terminus-quicksilver-plugin)
  - [Terminus Composer Plugin](https://github.com/pantheon-systems/terminus-composer-plugin)
  - [Terminus Drupal Console Plugin](https://github.com/pantheon-systems/terminus-drupal-console-plugin)
  - [Terminus Mass Update Plugin](https://github.com/pantheon-systems/terminus-mass-update)
  - [Terminus Aliases Plugin](https://github.com/pantheon-systems/terminus-aliases-plugin)
  - [Terminus CLU Plugin](https://github.com/pantheon-systems/terminus-clu-plugin)
- NPM
- Test tools
  - headless chrome
  - phpunit
  - bats
  - behat
  - php_codesniffer
  - hub
  - lab
- Test scripts

## Branches

- 6.x: Use a CircleCI base image with Node JS
- 5.x: Don't create multidevs when commits are made to the default branch, instead working directly on the dev environment
- 4.x: Terminus 2.x and Build Tools 2.x
- 3.x: Deprecated: Terminus 1 with Build Tools 2.0.0-beta2
- 2.x: Terminus 1.x and Build Tools 1.x
- 1.x: Deprecated
