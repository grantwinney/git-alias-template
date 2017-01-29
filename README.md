Git's "alias" feature provides a way for you to create shortcuts for other Git commands, which can save you a lot of time in the long run. If you want to learn more, [I wrote a bit about it here](https://grantwinney.com/what-is-a-git-alias-and-how-do-i-use-it/).

The [alias.gitconfig](alias.gitconfig) file in this repo is just a collection of some useful aliases I created, some for long git commands or chains of commands, and others for common typos.

If you'd like to use these aliases, you can clone the repository and reference it without doing anything funky to your existing gitconfig file, even leaving your existing aliases in place. Just run the following commands:

```
cd ~/your/projects
git clone git@github.com:grantwinney/git-alias-template.git
git config --global include.path "~/your/projects/git-alias-template/alias.gitconfig"
```

That inserts a new section in your gitconfig file (seen below), which imports settings from another file and merges its functionality without affecting the main config file.

```
[include]
    path = ~/your/path/to/projects/git-alias-template/alias.gitconfig
```

You can read more about Git aliases here:

* [GitHowTo: Aliases](https://githowto.com/aliases)
* [Pro Git: 2.7 Git Basics – Git Aliases](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases)

Do you have any especially useful aliases of your own that you couldn't live without? If you want to share them, feel free to [create a pull request](https://help.github.com/articles/creating-a-pull-request/) and I'll check them out.
