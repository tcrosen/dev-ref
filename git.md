# Git

Distributed source control.

## Commands

**Delete all local non-master branches**

```sh
$ git branch | grep -v "master" | xargs git branch -D 
```

**Squash all commits into a single commit**

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

## Common Problems

> I have XCode installed (and consequently it's bundled git); how do I get my system to use this version instead?

> Xcode installs it's git to /usr/bin/git; recent versions of OS X (Yosemite and later) ship with stubs in /usr/bin, which take precedence over this git. To overcome, do the following:

```sh
sudo mv /usr/bin/git /usr/bin/git-system
sudo ln -sf /usr/local/git/bin/git /usr/bin/git
```

## Resources

* [Dealing with Line Endings](https://help.github.com/articles/dealing-with-line-endings/)
* [Destroy your entire commit history](http://stackoverflow.com/questions/9683279/make-the-current-commit-the-only-initial-commit-in-a-git-repository)
