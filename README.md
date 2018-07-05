# GIT - Playground

This is collaboration of all resources, hands-on activities and experiences. This is not some code base, Purpose of 
this is to keep on learning git down the line and keep all resources at a safe place so it will be helpful further 
for relearn or troubleshoot purposes.

## Index - What all included

1. Cheatsheets
   - Atlassian Cheatsheet: A brief cheetsheet including main commands. [Altassian Cheatsheet](https://github.com/Ravi-Upadhyay/git-playground/blob/master/Cheatsheets/atlassian/atlassian-git-cheatsheet.pdf)
   - Git Tower Cheatsheet Bundle: A collection of cheatsheets, nicely structured. [Git Tower Cheatsheet](https://github.com/Ravi-Upadhyay/git-playground/tree/master/Cheatsheets/git-tower)
2. Markdown (.md) File Syntax
3. Submodules
4. Template - README.md file

### Cheatsheets

These cheatsheets contain basic to advance level git commands that will enable you to master/troubleshoot git. 
Git command line is very vast and advanced which may include several scenarios. While cheatsheet by Atlassian is 
handy one page to use on your normal day to day needs, Git tower has collection of documents to help get rid of 
any riddle that might come.

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

## Links - Other useful info over web

1. [Try github commands `a nice interface for hands on`](https://try.github.io)
2. [All about GIT `explore deep`](https://git-scm.com/book/en/v2)
3. [How to write readme files `syntax explanations`](https://help.github.com/articles/basic-writing-and-formatting-syntax/#lists)
4. [Readme.md template `that is how its done`](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)

