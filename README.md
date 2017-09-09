# Git Hook for using Commitizen Commit Types

Quick ```prepare-commit-msg``` hook that pre-appends two commented out lines to your Git commit message. Uncomment them
to use, or ignore and write your own.

Makes use of the JSON resource under [Commitizen's conventional-commit-types](https://github.com/commitizen/conventional-commit-types/).

## Requirement

Obviously uses ```Git```, not so obvious is this hook makes use of ```Node``` to parse through the JSON, it was just easier in the moment. Feel free to change.

## Install

Move/copy/whatever the ```prepare-commit-msg``` file to your repositories Git hooks directory. You may need to ```chmod```
the file.
