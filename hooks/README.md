# Git Hooks
[Git Hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) are used to enforce various checks while working with a git repository. PX Blue uses hooks to enforce consistency of commit messages while working on PX Blue resources and materials.

## Installation
You will need to clone this repository to a permanent location on your computer (the git config will refer to this location):
```
cd path/to/safelocation
git clone https://github.com/pxblue/.github
```

## Configuration
You can use these git hooks on a per-project basis using `git config`, but we recommend using these settings globally across all of your projects for ease of use.
```
git config --global core.hooksPath path/to/safelocation/.github/hooks
```
> **NOTE:** if you have multiple git profiles configured, you will need to run this command once for each profile. 

## Usage
These hooks will be automatically applied to any git projects on your computer. If you attempt to make a commit that violates one of the policies, you will be presented with an error message and required to make necessary changes before you can commit.
