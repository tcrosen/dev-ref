dev-ref
=======

Reference for development tasks/resources

#Git

###Undo all unstaged changes

`git clean -fd`

Dry run: `git clean -nd`

Also remove ignored files: `git clean -fdx`

###Undo commits that have not been pushed yet

`git reset HEAD~1`

Also undo current changes: `git reset --hard HEAD~1`

###Checkout a remote branch for an existing local repository

```
git fetch
git checkout test
```

#Angular

- [ngBoilerPlate](https://github.com/ngbp/ngbp) - Opinionated architecture for scalable Angular apps
- [Best Practices for App Structure](https://docs.google.com/document/d/1XXMvReO8-Awi1EZXAXS4PzDzdNvV6pGcuaF4Q9821Es/pub) *(Official)*
- [Code style guide](https://google-styleguide.googlecode.com/svn/trunk/angularjs-google-style.html)  *(Official)*


