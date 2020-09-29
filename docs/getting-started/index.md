---
title: Getting Started
has_children: true
nav_order: 2
---

# Getting Started

The Widget SDK is aimed at web developers who have knowledge about JavaScript, HTML and CSS. We recommend inline widgets to be built using TypeScript + Angular (2.x), as these techniques are used for the Homepages framework and application.

The Widget SDK zip file includes documentation (Developer's Guide and a Framework API reference), source code, Widget samples project and a simple NodeJS server to run the samples on if not using the included Visual Studio solution.
The latest Widget SDK deliverable can be found here.

## Tenant widgets
Tenant widgets are widgets developed by partners or customers for the cloud edition of Homepages. These pages describes the process for developing and "running" a tenant widget.

Tenant widgets can oly be used in the cloud edition of Homepages. There are some limitations and restrictions that applies to tenant widgets, for example the widget id must start with ‘tenant.’ and the manifest must have an author property specified. There is also a limit to the number of files that a tenant widget zip can contain when it is imported into a Homepages environment.

The sample “tenant.sample.angular.helloworld” is an example of a tenant widget.

## Prerequisites
To use all parts of the Homepages Widget SDK you will need Node.js, a TypeScript compiler and an Integrated development environment (IDE) or a Text Editor. Some of the possible alternatives are listed below.

<b> Node.js </b> 
  <br> https://nodejs.org/en/ <br>
<br><b> TypeScript </b> 
  <br> http://www.typescriptlang.org/
  <br> npm install -g typescript <br>
<br><b> Visual Studio Code (free) </b> 
  <br> https://code.visualstudio.com/ <br>
<br><b> Visual Studio Community (free) </b> 
  <br> https://www.visualstudio.com/vs/community/ <br>
<br><b> Visual Studio 2017 (license) </b> 
  <br> https://www.visualstudio.com/vs/ <br>


## Node.js dependencies
If you want to use any of the following parts of the SDK you need to install the Node.js dependencies. If you don't plan to use any of these you can just skip this step.

* <b>Angular</b> - Angular source code and typings matching the version used for Homepages.
* <b>Web server</b> - A simple development web server.
* <b>ION API Proxy</b> - A developmemt proxy for widgets that use the Infor ION API.
* <b>Homepages script</b> - Minify and pack widget into a production zip.

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

## Web server
The SDK includes a Node.js development web server that be used for viewing sample widgets and developing widgets. The web server is optional if you have another alternative such as the web server in Visual Studio. The web server will run on http://localhost:8080 by default and serve files from the "./Widgets" directory.

### Start web server in Visual Studio Code
Start the web server in Visual Studio Code by running the build task "Start Server" (ctrl+shift+b).

### Start web server with Windows command file
Use the StartServer.cmd command file to start the web server. Edit the command file to change the default port and path.
```
StartServer.cmd
```

### Start web server with npm
Use one of the following npm commands to start the web server. The port and path can be changed in the configuration section of the package.json file, see server_port and server_path.
```
npm start
```
```
npm run server
```

### Start web server with node
Use one of the following node commands to start the web server. The port and path can be provided as parameters. If no parameters are specified the default port 8080 and the default path "./Widgets" will be used
```
node server
```
```
node server 8080 "./Widgets"
```

## View samples
Once the web server is running you can view the default sample by navigating a browser to http://localhost:8080/index.html

### View samples with Windows command file
Use the OpenSamples.cmd command file to open the default sample in the default browser on Windows.
```
OpenSamples.cmd
```

## Compile samples
Compile all the TypeScript samples in Visual Studio Code by running the build task "Typescript Watch" (ctrl+shift+b). The files are watched, and will be recompiled automatically when saved. Refresh your browser to see the changes.

## ION API Proxy
When developing widget that use ION API you can use the included proxy. See the ION API samples in the Samples/Widgets directory for more information. You need to know the hostname and port of the ION API server to be able to configure the proxy.

### Start proxy with Windows command file
Start the proxy using the StartIonApiProxy.cmd command file. Make sure to edit the command and provide correct values for the local port, remote  host and port.
```
StartIonApiProxy.cmd
```

### Start proxy with npm
Use the following npm command to start the proxy. The local port, remote host and remote port can be changed in the configuration section of the package.json file, see proxy_local_port, proxy_remote_host and proxy_remote_port.
```
npm run proxy
```

### Start proxy  with node
Use the following node command to start the proxy. The local port, remote host and remote port and  should be provided as parameters.
```
node proxy 8083 "domain.server.com" 443
```

## Homepages command script
The homepages command script performs different commands. For the help documentation use:
```
node homepages help
```
### Package
Widgets have to be bundled (if consisting of multiple .ts files) and minified before delivery. The package command can be used to build, minify and package a widget or a list of widgets.
```
node homepages pack "infor.sample.helloworld"
```

## Read more
[Link to another page](widget-framework)
