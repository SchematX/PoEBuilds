
# Contributing to Path of Building

## [Reporting bugs] <- (https://github.com/SchematX/PoEBuilds/issues)

#### Before creating an issue:
* Check that the bug hasn't been reported in an existing issue. View similar issues on the left of the submit button.
* Make sure you are running the latest version of the build. Check back here hourly or nightly for updated Live builds in the past 24-48 hours
* If you've found an issue with any of our builds, please be sure to check our logs on the front page incase there has been an update.

#### When creating an issue:
* Please provide detailed instructions on how to reproduce the bug, if possible.
* Provide the build share code to a build that is affected by the bug, if possible. In the "Import/Export Build" tab, click "Generate", then "Share with Pastebin" and add the link to your post.

## Requesting features
Feature requests are always welcome which you can here https://feathub.com/SchematX/PoEBuilds. You must have a github account in order to do-so, its FREE! Note that not all requests will receive an immediate response.

#### Before submitting a feature request:
* Check that the feature hasn't already been requested. Look at all issues with titles that might be related to the feature.
* Make sure you are running the latest version of the program, as the feature may already have been added.

#### When submitting a feature request:
* Be specific! The more details, the better.
* Small requests are fine, even if it's just adding support for a minor modifier on a rarely-used unique.

## Contributing code

#### Before submitting a pull request:
* Familiarise yourself with the code base [here](docs/rundown.md) to get you started.
* There is a [Discord](https://discordapp.com/) server for **active development** on the fork and members are happy to answer your questions there.
  If you are interested in joining, send a private message to any of **SchematX#5391** and we'll send you an invite.

#### When submitting a pull request:
* **Pull requests must be made against the 'dev' branch**, as all changes to the code are staged there before merging to 'master'.
* Make sure that the changes have been thoroughly tested!

#### Setting up a development install
Note: This tutorial assumes that you are already familiar with Git and basic command line tools.

The easiest way to make and test changes is by setting up a development install, in which the program runs directly from a local copy of the repository:

 - Clone the repository using this command:

       git clone -b dev https://github.com/SchematX/PoEBuilds.git
 Here is a list of other tools I use:

 - [Notepad++](https://notepad-plus-plus.org/)
 - [PoB Community](https://pathofbuilding.community/)
 - [PoE-Profile](https://poe-profile.info/)


#### Keeping your fork up to date

Note: This tutorial assumes that you are already familiar with Git and basic command line tools.

Note: If you've configured a remote already, you can skip ahead to step 6.

1. Check your current remote repositories.

       git remote -v
2. Add a new remote repository and name it `upstream`.

       git remote add upstream https://github.com/PathOfBuildingCommunity/PathOfBuilding.git
3. Verify that adding the remote worked by running the last command again.

       git remote -v
4. Fetch all branches and their commits from upstream.

       git fetch upstream
5. Check out your local `dev` branch if you haven't already.

       git checkout dev
6. Merge all changes from `upstream/dev` into your local `dev` branch.

       git rebase upstream/dev
7. Push your updated branch to GitHub.

       git push -f origin dev

#### Setting up a development environment

Note: This tutorial assumes that you are already familiar with the development tool of your choice.

If you want to use a text editor, [Visual Studio Code] or notepad ++ however (https://code.visualstudio.com/) is recommended.
or [IntelliJ Idea Community](https://www.jetbrains.com/idea/) are recommended.
They are all free and open source.

