Development Reference Manual
=======

Quick reference for common development tasks/resources that I need from time to time.

#Git

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

**Reference links:**

* [Dealing with Line Endings](https://help.github.com/articles/dealing-with-line-endings/)
* [Destroy your entire commit history](http://stackoverflow.com/questions/9683279/make-the-current-commit-the-only-initial-commit-in-a-git-repository)

#Node

**Stop using `sudo`**

```
$ sudo chown -R $USER /usr/local/bin
$ sudo chown -R $USER /usr/local/lib/node_modules
```

**List npm package versions without dependencies**

```
npm list [-g] --depth=0
```

#Angular

- [ngBoilerPlate](https://github.com/ngbp/ngbp) - Opinionated architecture for scalable Angular apps
- [Best Practices for App Structure](https://docs.google.com/document/d/1XXMvReO8-Awi1EZXAXS4PzDzdNvV6pGcuaF4Q9821Es/pub) *(Official)*
- [Code style guide](https://google-styleguide.googlecode.com/svn/trunk/angularjs-google-style.html)  *(Official)*

#OSX

**Edit the hosts file**

```
sudo <editor> /private/etc/hosts
```


