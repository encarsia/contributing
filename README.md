# Contributing

If you want to contribute to a project and make it better, your help is very welcome. Contributing is also a great way to learn more about social coding on GitHub, new technologies and their ecosystems and how to make constructive, helpful bug reports, feature requests and the noblest of all contributions: a good, clean pull request.

## How to make a clean pull request

Look for a project's contribution instructions. If there are any, follow them.

## General walkthrough

### Prerequisites

- Create a personal fork of the project on GitHub.
  * Use the web interface
- Clone the fork on your local machine. Your remote repo on Github is called `origin`.
  * `git clone https://github.com/yourname/repo.git`
- Add the original repository as a remote called `upstream`.
  * [GitHub Help: Configuring a remote for a fork](https://help.github.com/articles/configuring-a-remote-for-a-fork/)
  * `git remote add upstream https://github.com/originaluser/repo.git`
- If you created your fork a while ago be sure to pull upstream changes into your local repository.
  * [GitHub Help: Syncing a fork](https://help.github.com/articles/syncing-a-fork/)
  * *fetch* + *upstream* or *pull* syncs the files on your local machine, *push* to commit changes to your remote fork:
    1. `git fetch upstream`
    2. `git checkout master`
    3. `git merge upstream/master`
    4. `git push`
- Create a new branch to work on! Branch from `dev(elop)` if it exists, else from `master`.
  * Give it a descriptive name to make your intentions clear.

### Your turn

- Implement/fix your feature, comment your code.
- Follow the code style of the project, including indentation.
- If the project has tests run them!
- Write or adapt tests as needed.
- Add or change the documentation as needed.
- Squash your commits into a single commit with git's [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.
  * HELP!
- Push your branch to your fork on GitHub, the remote `origin`.
- From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`!
- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.

### The aftermath

- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete
your extra branch(es).
- It is also safe to delete your fork as your code is now part of the original. If you want to keep your fork, make sure to sync your copy with the latest version (see above).

## Final note

And last but not least: Always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.

## More

* [How To Create a Pull Request on GitHub](https://www.digitalocean.com/community/tutorials/how-to-create-a-pull-request-on-github)
