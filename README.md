# intellij-better-direnv

![Build](https://github.com/Fapiko/intellij-better-direnv/workflows/Build/badge.svg)
[![Version](https://img.shields.io/jetbrains/plugin/v/19275-better-direnv.svg)](https://plugins.jetbrains.com/plugin/19275-better-direnv)
[![Downloads](https://img.shields.io/jetbrains/plugin/d/19275-better-direnv.svg)](https://plugins.jetbrains.com/plugin/19275-better-direnv)

<!-- Plugin description -->
This plugin adds direnv support to IntelliJ IDEs.

The plugin can be accessed via the Run Configuration settings. To enable it for a given Run Configuration, check the
`Enable Direnv` checkbox. If you want it to automatically `direnv allow` when updates to the .envrc file are detected,
check the `Trust .direnv` checkbox. Note that this should only be done for trusted projects.

Currently supported Run Configurations:
  - Java
  - Go


Unfortunately, each run configuration type needs to be added manually. New run configuration support can be added
by request.

<!-- Plugin description end -->

## Installation

- Using IDE built-in plugin system:

  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>Marketplace</kbd> > <kbd>Search for "
  intellij-better-direnv"</kbd> >
  <kbd>Install Plugin</kbd>

- Manually:

  Download the [latest release](https://github.com/Fapiko/intellij-better-direnv/releases/latest) and install it
  manually using
  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>⚙️</kbd> > <kbd>Install plugin from disk...</kbd>

## Building with docker
```
docker run --rm -it -v `pwd`:/tmp/work openjdk:11 sh

## Inside the container
cd /tmp/work
./gradlew build

## Once complete the plugin will be in the build/distributions directory
```

---
Plugin based on the [IntelliJ Platform Plugin Template][template].

[template]: https://github.com/JetBrains/intellij-platform-plugin-template
