# Git Hook for Using Commitizen Commit Types

Quick ```prepare-commit-msg``` hook that pre-appends two commented out lines to your Git commit message. Uncomment them
to use, or ignore and write your own.

Makes use of the JSON resource under [Commitizen's conventional-commit-types](https://github.com/commitizen/conventional-commit-types/), with a fallback using the JSON
resource within this repository.

## Requirement

Obviously uses ```git```, not so obvious is this hook makes use of ```Node``` to parse through the JSON, it was just easier in the moment. Feel free to change.

## Install

Move/copy/whatever the ```prepare-commit-msg``` file to your repositories Git hooks directory. You may need to ```chmod```
the file.

## Use

Once you've installed the hook ```$ git commit```... like you would normally. The hook will ask you a series of questions with similarities to Commitizen.

Basic commands:
- ```ctrl c``` to escape the entire Git sequence
- type ```q``` hit ```enter``` to quit the entire Git sequence
- type ```s``` hit ```enter``` to skip the question sequence and ```git``` on with it

As long as you're using some form of ```git``` CLI, and once you've answered the questions, you should see a couple of commented lines in your commit message (dependent on if you skipped them). You can choose to use these commented lines or ignore them and continue on your merry way.
