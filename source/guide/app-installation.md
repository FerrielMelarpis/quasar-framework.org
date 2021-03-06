title: Main Starter Kit Installation
---
Using the Main Starter Kit is the recommended way to go in order to benefit from all Quasar can do for it. You'll be able to build:
* a SPA (Single Page Application/Website),
* a PWA (Progressive Web App),
* a Mobile App (through Cordova),
* an Electron App,
...sharing the same base-code.

First, we install Quasar CLI. Make sure you have Node >=8 and NPM >=5 installed on your machine.

```bash
# Latest NodeJS is required.
$ npm install -g quasar-cli
```

Then we create a project folder with Quasar CLI:
```bash
$ quasar init <folder_name>
```

Note that you don't need separate starter kits if you want to build any of the options described above. This one can seamlessly handle all of them.

Make sure you familiarize yourself with the [Quasar CLI](/guide/quasar-cli.html) because you will be using it a lot.

## What's Included

While developing with Dev Server (`$ quasar dev`):
* Babel, so you can write ES6 code
* Webpack + vue-loader for Vue SFC (single file components)
* State preserving hot-reload
* State preserving compilation error overlay
* Lint-on-save with ESLint
* Source maps
* Develop right on a device emulator (or a real phone connected to your machine) if you target a Mobile App
* Develop right on an Electron window with Developer Tools included if you target an Electron App

Developing for production (`$ quasar build`):
* Javascript minified with [UglifyJS](https://github.com/mishoo/UglifyJS2)
* HTML minified with [html-minifier](https://github.com/kangax/html-minifier)
* CSS across all components extracted (and auto-prefixed) into a single file and minified with [cssnano](https://github.com/ben-eb/cssnano)
* All static assets are compiled with version hashes for efficient long-term caching, and a production index.html is auto-generated with proper URLs to these generated assets.

Take note of '/quasar.conf.js' file in the root of your project folder. This file helps you quickly configure the way your website/App works. We'll go over it in [Configuration](/guide/app-quasar-conf.html) section.
