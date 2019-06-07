# Quick guide to contributing to a github project

Ever wondered how to started with contributing to a GitHub project? This is the place for you.

[tldr](#tldr)

## Step-by-Step

### 1. Set up a working copy on your computer
* get a local `fork` of the project
    * press `fork` button in a github project
    * this will create a copy of the repository in your own github account
* get a localy copy: `git clone git@github.com:bgguna/kubecon-europe-2019-notes.git`
* go to the cloned repo: `cd kubecon-europe-2019-notes`
* set up a new remote that will point to the original project: `git remote add upstream git@github.com:kaushikchaubal/kubecon-europe-2019-notes.git`
* now you will have 2 remotes:
    * `origin` which points to your github fork
    * `upstream` which points to the original github project

### 2. Get it working on your machine

### 3. Add your changes
* create a local branch
```bash
git checkout  master
git pull upstream master && git push origin master
git checkout -b hotfix/readme-update
```
* the branch can be created from `develop` (for features) and/or `master` (for bugfixes), and can be prefixed with: `feature/`, `hotfix/`, `bug/`.
* commit your changes, following this [guide](https://www.conventionalcommits.org/en/v1.0.0-beta.4/)

### 4. Create the PR
* push your branch to the `origin` remote: `git push -u origin hotfix/readme-update
* go to your web version of the repo: https://github.com/bgguna/kubecon-europe-2019-notes
* hit `Compare & pull request`

### 5. Reviewing
* your changes will be reviewed by the maintainers, and if everything is ok, they will eventually be merged to the project

## TLDR
1. Fork the project & clone
2. Create upstream remote and sync your local copy from the original project
3. Branch out
4. Make and commit your changes
5. Push to your origin repo
6. Create a new pull-request
7. Respond to code review feedback

## Resources
* [The beginner's guide to contributing to a GitHub project](https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/), Rob Allen's DevNotes