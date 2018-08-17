---
title: Getting Started
description: Getting Started guide for Cogear.JS
layout: docs
js: ['js/docs.js','js/help.js']
---
# About
**Cogear.JS** is a static websites generator built with [Node.JS](https://nodejs.org) and based on [Webpack](https://webpack.js.org) (v4.6).

It's inspired by [Jekyll](https://jekyllrb.com) and others, but built on the top of the latest frontend technologies.

Providing awesome experience of on-the-fly hot reloading to instantly implementing any changes.

<article class="message is-info is-desktop">
  <div class="message-body">Use arrow keys <button>&larr;</button> <button>&rarr;</button> to navigate through the docs.</div>
</article>

## Features
* It can be usefull for building modern static websites (using [Vue.JS](https://vuejs.org), [React](https://reactjs.org), [Angular](https:/angular.io), [Ember](https://emberjs.org)) or even for rapid prototyping.
* It's **blazing fast and reliable** being online. Server can handle thousands requests per seconds to serve static files (even on tiny VPS).
* It doesn't requires **any database** and works on **every hosting** (as it produces *static html and assets files*).
* It's **100% secure** for hacking because it has no backend after being deployed to the server.
* It can use **any modern frontend stack** because it uses **Webpack** in system core.

Using [Github Pages](https://pages.github.com) (or any similar project) you can host generated site **for free**.

### What it can be used for:
* Rapid site prototyping, 
* Portfolio site,
* Company site,
* Product site,
* Personal blog,
* Artist or musician site.

Any site that has its administrator generated content.

Using [Firebase](https://firebase.google.com) or any other _backend_, written in _any lang_ (**PHP**, **Ruby**, **Python**, **Node.JS**) or even with CMS like a **WordPress**, with help of modern frontend technologies like [Vue.JS](https://vuejs.org) or [React](https://reactjs.org), it can be turned into more dynamic site like **e-commerce**, **products catalog** and so on.

### What it cannot be used for:
* Forum,
* Social network,
* Chat.

Or any other site type with great amount of user-generated content which relies on heavily database usage and dynamically generated pages.

# Requirements

You have [Node.JS](https://nodejs.org) (9.x or higher) and [NPM](https://www.npmjs.com) (usually comes together) to be installed.

[Download and install](https://nodejs.org/en/download/)

The latest version (v10.9.0) is recommended.

**Cogear.JS** runs on:
* Mac
* Linux
* Windows

You may also want to use awesome [VSCode](https://code.visualstudio.com) editor.

# Installation
To install **Cogear.JS** do next:
```bash
> npm install cogear -g
# or
> yarn global add cogear
```
Done. Congratulations! 

**Cogear.JS** is now available by CLI-command `cogear`.

Now you're ready to build your first site.

# Usage
Go to the directory where all your local sites are hosted.
```bash
> cd ~/Sites
```
Create a new site via command:
```bash
> cogear new awesome-static-site # where "site" is your site folder name

# if you have a preset, use it's git repo address as fourth arg
> cogear new awesome-static-site https://github.com/codemotion/cogear-preset-docs
```

After that go to site dir:
```bash
cd ~/Sites/awesome-static-site
```
And start up **Cogear.JS** in prefered mode.
```bash
> cogear # run in develompent mode with hot-reload – by default

> cogear build # build a site

> cogear production # build a site and run local server

> cogear deploy # deploy site to the default server
```
# Options
All available options can be seen via `--git` (or shortcut `-h`) command.
```bash
> cogear -h

╓─────────────────────────────────────────────────────────────╖
║                                                             ║
║                                                             ║
║        Cogear.JS – modern static websites generator.        ║
║                                                             ║
║                    https://cogearjs.org                     ║
║                                                             ║
╙─────────────────────────────────────────────────────────────╜

Usage: cogear [command]

Runs in development mode by default (without [command]).

Options:

  -h, --help          output usage information
  -s, --src           set source directory, default: ./src
  -o, --output        set output directory, default: ./public
  -h, --host          set host for local server, default: localhost
  -p, --port          set port for local server, default: 9000
  -o, --open          if set to false, browser will not be opened after build, default: false
  -v, --version       print current version
  -w, --verbose       set webpack verbose mode, default: true

Commands:

  command   (alias)     [optional]      description

  [dev]        (d)                     run dev server # hot-reload for pages, scripts, styles [DEFAULT]
  production   (p)                     run build and starts static server
  build        (b)                     run build
  deploy       (d)       [preset]      deploy site to server
  new          (n)       [site-name]   generate new site
  plugin       (p)       [plugin-name] generate plugin boilerplate
  theme        (t)       [theme-name]  generate theme boilerplate

For more information visit:
https://cogearjs.org
```
Let's take a look at the workflow.