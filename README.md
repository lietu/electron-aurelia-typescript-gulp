# Aurelia powered Electron application with Gulp and TypeScript

This is a skeleton application to get started with developing Aurelia powered
Electron applications, using Gulp to deal with compilation etc.

What does all that mean?

It means you can develop cross-platform desktop applications using modern
web application technologies.

 - HTML5
 - SCSS + CSS3
 - TypeScript

The different components used in this skeleton are:

 - [Aurelia](http://aurelia.io/) is a modern web application framework
 - [Electron](http://electron.atom.io/) makes cross-platform desktop apps powered with web technologies
 - [TypeScript](http://www.typescriptlang.org/) modern programming language that compiles into plain JavaScript
 - [SCSS](http://sass-lang.com/) is a modern version of CSS that makes working with CSS much more enjoyable and compiles to plain CSS.
 - [Gulp](http://gulpjs.com/) automates workflows and reduces need for IDE integration and shell scripts


## Why?

Well, this question is really 4-fold.


### Why Aurelia?

It's pretty neat. You can write in TypeScript, and the code you write for it is 
clean.
 
 
### Why Electron?

Electron seems to be the only mature framework for creating cross-platform 
desktop applications using HTML, CSS and JavaScript.


### Why Gulp?
 
Gulp makes your development process not depend on specific IDEs and
configuration, and is still quite flexible vs. e.g. bower.


### Why should you use this skeleton?

Aurelia is a bit of a pain to set up, TypeScript is a bit of a pain to set up,
Electron is a bit of a pain to set up, and getting all that to work with Gulp
is a lot of pain to set up.

This provides you a way to get over a lot of headaches and just get to work on
your application.


## How to use this?

### Prerequisites

You will need at least the following installed:

 - [Node.js with NPM](https://nodejs.org/en/)


### Setup

Setting up the dependencies once you have a clone of this repo is easy:

```
npm install -g gulp jspm
npm install
jspm endpoint config github
jspm install -y
```

The `jspm endpoint config github` command will ask for you to set up a token
to GitHub. It will need to have `public_repo` access, to bypass GitHub rate
limiting that will kill the installation of all the dependencies.


### Running

Firstly have a terminal open where you have gulp running to detect the changes
to your code and automatically compile them to the `dist/` -folder.

```
gulp
```

Then open up another terminal where you launch the app from:

```
cd dist
electron launcher.js
```
 
 
## Update Aureliel etc.

This repo might get old, but it should be easy to update relevant stuff as long
as there aren't ginormous changes to how the various components operate.

To update the NPM dependencies:

```
npm install -g npm-check-updates
ncu -u
npm install
```

To update the Auriel framework + deps to latest version:

```
jspm dl-loader --latest
```


# Financial support

This project has been made possible thanks to [Cocreators](https://cocreators.ee) and [Lietu](https://lietu.net). You can help us continue our open source work by supporting us on [Buy me a coffee](https://www.buymeacoffee.com/cocreators).

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/cocreators)
