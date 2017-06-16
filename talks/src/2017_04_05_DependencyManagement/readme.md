# Dependency Management for Javascript & asp.net

## Introduction
“The primary function of any package manager is to install some package – a piece of code that serves a particular purpose – from a global registry into an engineer‘s local environment. Each package may or may not depend on other packages. A typical project could have tens, hundreds, or even thousands of packages within its tree of dependencies.”

>*Yarn: A new package manager for JavaScript*<br/>
``https://code.facebook.com/posts/1840075619545360/yarn-a-new-package-manager-for-javascript/``


## Demo Goal
Presenting a simple demonstration for a web-development stack with **node.js (npm)** and **yarn**

### Final Demo Stack
> node.js <-> npm <- yarn -> jquery

## Demo Workflow
### Setup
1. Download and install Node.js https://nodejs.org/en/
2. Update npm from command prompt: `` npm install npm@latest -g``
3. Install Yarn: ``npm install --global yarn``

### Run yarn from project directory
> More infos: ``https://yarnpkg.com/en/docs/usage``

- Initialize a new Yarn project: ``yarn init``
- Add package to dependencies: ``yarn add {pkgName}``
- Add js dependency to html: ``node_modules/{pkgName}/dist/{pkgName}.min.js"``

### Finished demo index.html source
```
    <!DOCTYPE html>
    <html lang="en">
        <head>
            <title>Dependency Management for Javascript and asp.net - Demo</title>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1">
            <script src="node_modules/jquery/dist/jquery.min.js"></script>
        </head> 
        <body>
            <button id="btn" type="">Click me!</button>
            <h1 style="display: none;">It works</h1>

            <script>
                console.log("foobar");
                $("#btn").click(function(){
                    $("h1").toggle();
                });
            </script>
        </body>
    </html>
```

### Have fun!

## Useful *Visual Studio Code* Extensions
### Html5 Snippets
Provides html5 snippets

>``https://marketplace.visualstudio.com/items?itemName=abusaidm.html-snippets``

### Yarn
Provides the yarn commands for your project

> ``https://marketplace.visualstudio.com/items?itemName=gamunu.vscode-yarn``

## Relevant Links

### Package Managers
#### Yarn - *Fast, reliable, and secure dependency management.*
>``https://yarnpkg.com/en/``
#### NPM - *Build amazing things*
> ``https://www.npmjs.com/``
#### Nuget - *Everything you need for .net development*
> ``https://www.nuget.org/``
#### Bower - *A package manager for the web*
> ``https://bower.io/``

### Server-Side
#### Nodejs - *A JavaScript runtime built on Chrome's V8 JavaScript engine*
- ``http://nodejs.org``

#### asp.net Core - *A lean and composable framework for building web and cloud applications.*
- ``https://www.asp.net/core/``

#### asp.net - *An open source web framework for building modern web apps and services with .Net.*
- ``https://www.asp.net/``

## Moar Links!!!
Yarn: A new package manager for JavaScript
> ``https://code.facebook.com/posts/1840075619545360/yarn-a-new-package-manager-for-javascript/``

NPM or Yarn? Node.js devs pick their package manager
> ``http://www.infoworld.com/article/3172725/javascript/npm-or-yarn-nodejs-devs-pick-their-package-manager.html``
 
npm on **alternativeTo - *Crowdsourced software recommendations***
> ``http://alternativeto.net/software/npm/``

Thoughts on the npm fiasco
> ``https://www.akawebdesign.com/2016/03/25/thoughts-npm-fiasco/``

When to use Yarn over NPM? What are the differences?
> ``http://stackoverflow.com/questions/40027819/when-to-use-yarn-over-npm-what-are-the-differences``
