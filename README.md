# GIT - Playground

This is collaboration of all resources, hands-on activities and experiences. This is not some code base, Purpose of 
this is to keep on learning git down the line and keep all resources at a safe place so it will be helpful further 
for relearn or troubleshoot purposes.

## Index - What all included

- Cheatsheets
   - Atlassian Cheatsheet: A brief cheetsheet including main commands. [Altassian Cheatsheet](https://github.com/Ravi-Upadhyay/git-playground/blob/master/Cheatsheets/atlassian/atlassian-git-cheatsheet.pdf)
   - Git Tower Cheatsheet Bundle: A collection of cheatsheets, nicely structured. [Git Tower Cheatsheet](https://github.com/Ravi-Upadhyay/git-playground/tree/master/Cheatsheets/git-tower)
- Merge
- Stash
- Revert
- Markdown (.md) File Syntax
- Submodules
- Template - README.md file

### Cheatsheets

These cheatsheets contain basic to advance level git commands that will enable you to master/troubleshoot git. 
Git command line is very vast and advanced which may include several scenarios. While cheatsheet by Atlassian is 
handy one page to use on your normal day to day needs, Git tower has collection of documents to help get rid of 
any riddle that might come.

### Merge

Merging is Git's way of putting a forked history back together again. The git merge command lets you take the independent lines of development created by git branch and integrate them into a single branch.

[A nice explaination, Git Merge](https://www.atlassian.com/git/tutorials/using-branches/git-merge)

//TODO: continue

### Stash

Often, when you’ve been working on part of your project, things are in a messy state and you want to switch branches for a bit to work on something else. The problem is, you don’t want to do a commit of half-done work just so you can get back to this point later. 

1. Use `git stash` to push new stash onto your stack.
2. Now your working directory will be clean, you can switch to another branches as well.
3. You can use `git stash list` to see the list of all stashes. For example: _example-stash-1_
4. Use `git stash apply` to bring all changes back to working directory, top most stash.
5. Use `git stash apply <stash>` to bring all changes back to working directory, stash whichever mentioned. For example: _example-stash-2_

```

// EXAMPLE-STASH-1: get list of all stashes

$ git stash list
stash@{0}: WIP on master: 049d078 added the index file
stash@{1}: WIP on master: c264051 Revert "added file_size"
stash@{2}: WIP on master: 21d80a5 added number to log

// EXAMPLE-STASH-2: apply stash to particular stash 

$ git stash apply stash@{2}


```

### Revert

The git revert command can be considered an 'undo' type command, however, it is not a traditional undo operation. Instead of removing the commit from the project history, it figures out how to invert the changes introduced by the commit and appends a new commit with the resulting inverse content.

[A nice explaination, Git Revert](https://www.atlassian.com/git/tutorials/undoing-changes/git-revert)

### Markdown

Please find link below to learn more about how to write markdown files. The purpose of writing markdown files is
they are simple and can contain wide variety of information that may need for present some document about any repository
or project.

### Submodules

* The purpose of git submodules is to have an independent another git repository within a git repository.
* Suppose, in your project you have some submodule which exists as an independent git repository or project. A plugin may be.
* Another use which I see to manage git account by clubbing similar set of repository. (i.e. some ES6 repo may be part of JS).

#### Submodules - How it works ?

1. To add any repository as submodule, clone it inside repository normally `git clone https://github.com/repo-sub-module.git`
2. Use `git status` you will be able to see added repository as `untracked folder/files`
3. Instead of using `git add repo-sub-module` use `git submodule add https://github.com/repo-sub-module.git`
4. Now it has been added as submodule and a new file will be generated `.gitmodules`. Which will keep info about sub modules.
5. Note that now it is independent submodule. It can independently progress. 
6. If some changes have been made in submodule. You have to pull submodule to local and then merge/commit in submodule directory as well as parent directory.
7. Only commiting on parent's git will not affect submodule's git.
8. While cloning parent if you want to clone submodules also use `git clone --recursive https://git-hub.com/parent-repo-with-sub-modules.git`
9. When you go into submodule directory, you will find `HEAD` in `detached` state. You can `git checkout master` to `attach HEAD` to branch.

### Try GIT - Some handson exersice

There are some great tools available to help you in learning process. Best things they offer are

- Visulaization of every step.
- Minimal, to keep focused over one activity at a time.
- You can choose your own pace.

1. [Visualize GIT, A best way to try](http://git-school.github.io/visualizing-git/)
2. [Visualize GIT, branching](https://learngitbranching.js.org/?NODEMO)
3. [Tutorial of GIT commands, Levels](https://learngitbranching.js.org)

### Templates

Some templates that are ready to use and will give ideas about best practices to follow:

1. [Readme.md template `that is how its done`](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)

## Links - Other useful info over web

1. [Try github commands `a nice interface for hands on`](https://try.github.io)
2. [All about GIT `explore deep`](https://git-scm.com/book/en/v2)
3. [How to write readme files `syntax explanations`](https://help.github.com/articles/basic-writing-and-formatting-syntax/#lists)

