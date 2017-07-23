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


## Node


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

## Angular

- [ngBoilerPlate](https://github.com/ngbp/ngbp) - Opinionated architecture for scalable Angular apps
- [Best Practices for App Structure](https://docs.google.com/document/d/1XXMvReO8-Awi1EZXAXS4PzDzdNvV6pGcuaF4Q9821Es/pub) *(Official)*
- [Code style guide](https://google-styleguide.googlecode.com/svn/trunk/angularjs-google-style.html)  *(Official)*

## OSX

**Edit the hosts file**

```
sudo <editor> /private/etc/hosts
```

## Sublime Text 2

- [Settings](sublime-settings.json)
