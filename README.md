# Uix Create React App


[![Travis CI](https://img.shields.io/travis/com/xizon/uix-create-react-app?style=for-the-badge)](https://travis-ci.com/xizon/uix-create-react-app/)
[![npm version](https://img.shields.io/npm/v/uix-create-react-app?style=for-the-badge)](https://www.npmjs.com/package/uix-create-react-app)
[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=for-the-badge)](LICENSE)


## Demo

[https://xizon.github.io/uix-create-react-app/examples/](https://xizon.github.io/uix-create-react-app/examples/)



## Table of Contents


* [Description](#description)
* [Installation And Test](#installation-and-test)
* [File Structures](#file-structures)
* [Contributing](#contributing)
* [Changelog](#changelog)
* [Licensing](#licensing)



## Description

A set of React tool and scaffold. 

**Access your application without a server.**


* * *


## Installation And Test

You will need to have [node](https://nodejs.org/) setup on your machine. That will output the built distributables to `./dist/*` and `./examples/*.html`.


**Step 1.** Use NPM (Locate your current directory of project, and enter the following command.) or download the latest version from [Github](https://github.com/xizon/uix-create-react-app). For nodejs you have to install some dependencies.

```sh
$ sudo npm install uix-create-react-app
```

Or clone the repo to get all source files including build scripts: 

```sh
$ git clone git://github.com/xizon/uix-create-react-app.git
```


**Step 2.** First, using an absolute path into your `"uix-create-react-app/"` folder directory.

```sh
$ cd /{your_directory}/uix-create-react-app
```


**Step 3.** Before doing all dev stuff make sure you have `Node 14+` installed. After that, run the following code in the main directory to install the node module dependencies.

```sh
$ sudo npm install
```

**Step 4.** Commonly used commands:

Debug application. It can be checked separately as TypeScript without compiling and packaging behavior.

```sh
$ npm run check
```

To use webpack to bundle files. The converted ES5 files will be created.

```sh
$ npm run build
```

Using `Ctrl + C` to stop it.


**Step 5.** When you done, this will spin up a server that can be accessed at

```sh
http://localhost:8080/examples/
```


**Step 6 (Optional).** Run the following command to test(No packaging behavior), and used for TypeScript file inspection and debugging:

```sh
$ npm run dev
```


**Step 7 (Optional).** Unit Testing

```sh
$ npm run test
```




### ?????? Note:
 
**a) ERROR: npm update check failed.**

Solution:

```sh
$ sudo chown -R $USER:$(id -gn $USER) /Users/{username}/.config
```

**b) ERROR: Node sass version 6.x.x is not compatible with ^ 4.x.x.**

Solution:

```sh
$ npm install node-sass@4.14.1
```


**c) If you upgrade the version of Node, please execute the following code:**

```sh
$ sudo npm install
$ sudo npm rebuild node-sass
```

**d) Some compilation errors of TypeScript:**


Install TypeScript and ts-node globally on your machine

```sh
$ sudo npm install -g typescript ts-node
```



### ?????? Site Info Configurations:

You can update the Placeholders in Templates by modifying the Site Info configuration of `package.json`. Like this:

```json
{
  "author": "UIUX Lab",
  "name": "uix-create-react-app",
  "email": "uiuxlab@gmail.com",
  "version": "1.0.0",
  "projectName": "Uix Create React App",
  "createdInfo": "UIUX Lab (https://uiux.cc)",
  "projectURL": "https://uiux.cc",
  "description": "A set of React tool and scaffold.",
  ...
}
```




### ?????? Custom import third-party library:

The application loads some third-party libraries (icons, animations, 3D engines, etc.) by default, you can load them as needed, or modify the configuration file. Access to `src/client/components/_plugins/`





* * *


## File Structures



```sh

uix-create-react-app/
????????? README.md
????????? CHANGELOG.md
????????? CONTRIBUTING.md
????????? LICENSE
????????? webpack.config.js
????????? package-lock.json
????????? package.json
????????? dist/
???   ????????? css/
???   ???   ????????? app.css
???   ???   ????????? app.css.map
???   ???   ????????? app.min.css
???   ???   ????????? app.min.css.map
???   ????????? js/
???   ???   ????????? app.js
???   ???   ????????? app.js.map
???   ???   ????????? app.min.js
???   ???   ????????? app.min.js.map
????????? src/
???   ????????? index.js
???   ????????? router/
???   ????????? components/   #Independent React components
???   ????????? views/
???   ???   ????????? _pages/
???   ???   ????????? _html/
????????? examples/
?????????
```



## Contributing

Finding bugs, sending pull requests or improving our docs - any contribution is welcome and highly appreciated. To get started, head over to our [contribution guidelines](CONTRIBUTING.md). Thanks!


## Changelog

[releases](CHANGELOG.md)



## Licensing

Licensed under the [MIT](https://opensource.org/licenses/MIT).

