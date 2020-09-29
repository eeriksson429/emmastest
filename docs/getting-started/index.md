---
title: Getting Started
has_children: true
nav_order: 2
---

# Getting Started

The Widget SDK is aimed at web developers who have knowledge about JavaScript, HTML and CSS. We recommend inline widgets to be built using TypeScript + Angular (2.x), as these techniques are used for the Homepages framework and application.

## Download the Widget SDK
The Widget SDK zip file includes documentation (Developer's Guide and a Framework API reference), source code, Widget samples project, SoHo Xi Directives sample project and a simple NodeJS server to run the samples on if not using the included Visual Studio solution.
The latest Widget SDK deliverable can be found here.

## Tenant widgets
Tenant widgets are widgets developed by partners or customers for the cloud edition of Homepages. These pages describes the process for developing and "running" a tenant widget.

Tenant widgets can oly be used in the cloud edition of Homepages. There are some limitations and restrictions that applies to tenant widgets, for example the widget id must start with ‘tenant.’ and the manifest must have an author property specified. There is also a limit to the number of files that a tenant widget zip can contain when it is imported into a Homepages environment.

The sample “tenant.sample.angular.helloworld” is an example of a tenant widget.
