# Git Hook for using Commitizen Commit Types

Quick ```prepare-commit-msg``` hook that pre-appends two commented out lines to your Git commit message. Uncomment them
to use, or ignore and write your own.

Makes use of the JSON resource under [Commitizen's conventional-commit-types](https://github.com/commitizen/conventional-commit-types/), with a fallback using the JSON
resource within this repository.

## Requirement

Obviously uses ```Git```, not so obvious is this hook makes use of ```Node``` to parse through the JSON, it was just easier in the moment. Feel free to change.

## Install

Move/copy/whatever the ```prepare-commit-msg``` file to your repositories Git hooks directory. You may need to ```chmod```
the file.

## Use

Once you've installed the hook ```$ git commit```... like you would normally. The hook will ask you a series of questions with similarities to Commitizen. To escape the sequence either ```ctrl c``` or type ```q``` and hit enter on one of the questions.

Basic commands:
- ```ctrl c``` to escape the entire Git sequence
- type ```q``` and hit ```enter``` to quit the entire Git sequence
- type ```s``` can hit ```enter``` to skip the question sequence and ```Git``` on with it

As long as you're using some form of Git on the CLI, and once you've answered the questions, you should see a couple of commented lines in your commit message (dependent on if you skipped them), you can choose to use them or ignore them, and continue on your merry way.
