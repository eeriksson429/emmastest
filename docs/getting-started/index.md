---
title: Getting Started
has_children: false
nav_order: 2
---

# Getting Started

This section includes a brief quick start guide to the Homepages Widget SDK. For full instructions, please refer to the [Developer’s Guide](https://github.com/infor-cloud/homepages-widget-sdk/blob/master/DevelopersGuide.pdf).

## For who?

The Widget SDK is aimed at web developers who have knowledge about JavaScript, HTML and CSS. We recommend inline widgets to be built using TypeScript + Angular (2.x), as these techniques are used for the Homepages framework and application.

## What's Included

The Widget SDK zip file includes documentation (Developer's Guide and a Framework API reference), source code, Widget samples project and a simple NodeJS server to run the samples on if not using the included Visual Studio solution. The latest Widget SDK deliverable can be found [here](https://github.com/infor-cloud/homepages-widget-sdk).

## Dependencies
To use all parts of the Homepages Widget SDK you will need [Node.js](https://nodejs.org/en/), a [TypeScript compiler](http://www.typescriptlang.org/) and an [Integrated development environment or a Text Editor](https://code.visualstudio.com/). 

This section briefly describes how to quick start your widget development using the Homepages Widget SDK. Detailed instructions can be found in the [Developer's Guide](https://github.com/infor-cloud/homepages-widget-sdk/blob/master/DevelopersGuide.pdf).

## Node.js dependencies
If you want to use any of the following parts of the SDK you need to install the Node.js dependencies. If you don't plan to use any of these you can just skip this step.

* Angular - Angular source code and typings matching the version used for Homepages.
* Web server - A simple development web server.
* ION API Proxy - A developmemt proxy for widgets that use the Infor ION API.
* Homepages script - Minify and pack widget into a production zip.

### Install with npm
Run the following command in the Samples directory to install the Node.js dependencies.
```
npm install
```
### Install with Windows command file
Run the Install.cmd command file in the Samples directory to install the Node.js dependencies.
```
Install.cmd
```

## Widget sample code
To get an overview of the widget sample code you can open it in your development environment.

### Visual Studio Code
Start Visual Studio Code and use File > Open Folder and navigate to Samples/Widgets.
