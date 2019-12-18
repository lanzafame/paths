[![Build Status][travis-badge]][travis-link]
[![Slack Room][slack-badge]][slack-link]

# Paths

Create or append to environment variables.

## Install

With [fisherman]

```
fisher paths
```

## Usage

Create or overwrite environment variables.

```fish
echo VALUE > $paths_config/VAR
```

Create or append to environment variables.

```fish
mkdir $paths_config/VAR
echo VALUE > $paths_config/VAR/KEY
```

Where KEY is the name of the file that stores VAR's value and can be any name you wish.

When you're done, restart any open terminal sessions for the change to take effect.

### Examples

Set $EDITOR.

```fish
echo vim > $paths_config/EDITOR
```

Append to $PATH.

```fish
mkdir $paths_config/PATH
echo $GOPATH/bin > $paths_config/PATH/GOBIN
```

[travis-link]: https://travis-ci.org/fisherman/paths
[travis-badge]: https://img.shields.io/travis/fisherman/paths.svg
[slack-link]: https://fisherman-wharf.herokuapp.com
[slack-badge]: https://fisherman-wharf.herokuapp.com/badge.svg
[fisherman]: https://github.com/fisherman/fisherman
