Development Reference Manual
=======

Quick reference for common development tasks/resources that I need from time to time.

* [Git](#git)
* [Node](#node)
  - [npm](#npm)
* [Angular](#angular)
* [OSX](#osx)
* [Sublime Text 2](#sublime-text-2)
  - [Settings](sublime-settings.json)

##Git

**Use Atom as default editor**

```sh
$ git config --global core.editor "atom --wait"
```

**Squash commits into a single commit**

```sh
$ git rebase -i [--root]
```

**Undo all unstaged changes**

```
$ git clean -fd
```

Also remove ignored files: 

```
$ git clean -fdx
```

**Undo commits that have not been pushed yet**

```
$ git reset HEAD~1
```

Also undo current changes: 

```
$ git reset --hard HEAD~1
```

**Checkout a remote branch for an existing local repository**

```
git fetch
git checkout <branch name>
```

**Change a remote URL**

```
git remote set-url origin {new url}
```

**Delete a Tag**

```
# local
git tag -d {tag}

# remote
git push origin :refs/tags/{tag}
```

**Update Git version**

> I have XCode installed (and consequently it's bundled git); how do I get my system to use this version instead?

> Xcode installs it's git to /usr/bin/git; recent versions of OS X (Yosemite and later) ship with stubs in /usr/bin, which take precedence over this git. To overcome, do the following:

```sh
sudo mv /usr/bin/git /usr/bin/git-system
sudo ln -sf /usr/local/git/bin/git /usr/bin/git
```

**Reference links:**

* [Dealing with Line Endings](https://help.github.com/articles/dealing-with-line-endings/)
* [Destroy your entire commit history](http://stackoverflow.com/questions/9683279/make-the-current-commit-the-only-initial-commit-in-a-git-repository)

##Node


### npm

- [Fixing npm Permissions](https://docs.npmjs.com/getting-started/fixing-npm-permissions)

**Stop using `sudo`**

```
$ sudo chown -R $USER /usr/local/bin
$ sudo chown -R $USER /usr/local/lib/node_modules
```

**List npm package versions without dependencies**

```
npm list [-g] --depth=0
```

##Angular

- [ngBoilerPlate](https://github.com/ngbp/ngbp) - Opinionated architecture for scalable Angular apps
- [Best Practices for App Structure](https://docs.google.com/document/d/1XXMvReO8-Awi1EZXAXS4PzDzdNvV6pGcuaF4Q9821Es/pub) *(Official)*
- [Code style guide](https://google-styleguide.googlecode.com/svn/trunk/angularjs-google-style.html)  *(Official)*

##OSX

**Edit the hosts file**

```
sudo <editor> /private/etc/hosts
```

##Sublime Text 2

- [Settings](sublime-settings.json)
