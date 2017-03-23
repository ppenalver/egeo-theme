

<div align="center">
<img src="https://github.com/Stratio/egeo-web/blob/master/src/assets/images/egeo_logo_c.png">
</div>

# Egeo theme

Egeo Theme is a theme to work with [Egeo](https://github.com/Stratio/egeo), the Stratio's componente library to build interfaces.

In this repository, you'll find the CSS to put an skin over the Egeo components but this is only one part of the project. You can discover more in:

* [egeo](https://github.com/Stratio/egeo): The egeo library of components.
* [egeo-web](https://github.com/Stratio/egeo-web): The official website of Egeo where documentation will be available soon.
* [egeo-ui-base](https://github.com/Stratio/egeo-ui-base): A Sass library that helps us to build our styles, including a rewritten Sass version of [flexboxgrid](http://flexboxgrid.com/).
* [egeo-starter](https://github.com/Stratio/egeo-starter): A Boilerplate project prepared for work with Egeo 1.x, Angular 2.x, TypeScript, Webpack, Karma, Jasmine and Sass.

## Table of contents

* [About this repo](#about-this-repo)
* [File Structure](#file-structure)
* [Getting Started](#getting-started)
   * [Dependencies](#dependencies)
   * [Installing](#installing)
   * [Work with the code](#work-with-the-code)
   * [How to run](#how-to-run)
   * [How to test](#how-to-test)
   * [How to build](#how-to-build)
* [Contributing](#contributing)
* [License](#license)

## About this repo

This repository contains necesary .scss files to load different fonts, component skins and the grid used in Stratio's applicacions as well as the font files used in differents formats (.eot, .svg, .woff and .ttf)

* Documentation website (soon)

## File Structure

```
egeo-theme/
 ├──assets/                        * assets needed by the theme
 |   └──fonts/                     * fonts used
 |       └──font-folder/           * each font folder
 |           └──font-files         * eot, woff, otf, svg
 │
 ├──src/                           * the theme code
 |   ├──components/                * css rules applied for each Egeo component
 |   ├──settings/                  * settings of the theme
 |       ├──fonts.scss             * settings to work with fonts
 |       └──index.scss             * to load the whole settings
 |   ├──vendors/                   * 3rd party utilities, font css definitions...
 |       └──fonts/                 * fonts used
 |           └──font-name.scss     * each @font-face and css definition 
 |   ├──grid.scss                  * grid generator
 |   └──index.ts                   * to load the whole vendors
 │
 ├──.sass-lint.yml                 * our sass linting configuration
 ├──jenkinsfile                    * configuration of our jenkins process
 ├──pom.xml                        * configuration to work with our CI system
 ├──package.json                   * what npm uses to manage it's dependencies
 └──yarn.lock                      * need in order to get consistent installs across machines using yarn

```

## Getting Started

### Dependencies

What you need to run this app:
* [`node`](https://nodejs.org/es/) and `npm`
* Ensure you're running the latest versions Node `v6.x.x` and NPM `4.x.x`+

### Installing

You can install egeo-theme from npm:

```
npm i @stratio/egeo-theme
```

### Work with the code

You can use Npm or Yarn to work with egeo-theme. If you want to use Yarn, it has to be installed first as a global dependency in your local machine.

```
sudo npm i -g yarn
```

Once Yarn is installed or Npm is ready, you can install egeo-theme using:

```
yarn
```

or

```
npm install
```

### How to run

If you want to generate the final css, execute:

```
npm run build
``` 

or

```
yarn build
``` 

This generate four files, theme and grid minified and without minified.

### How to Test

There is a command to start the karma server and launch the whole tests written for the librery.

```
yarn test
```

or

```
npm run test
```

### How to Build

If you want to build a distributable package you must use the `build` command. This will create the css and minified css files in the root folder.

```
yarn build
```

or

```
npm run build
```
## Contributing

There are many ways to contribute to the egeo-theme project. [Check our contribution section in the Wiki to learn more](https://github.com/Stratio/egeo-theme/wiki/How-to-contribute).

## License

Egeo-theme is distributed under the Apache 2 license. You may obtain a copy of the license here at:

[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)
