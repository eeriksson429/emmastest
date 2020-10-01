---
title: Best Practices
has_children: false
nav_order: 3
---

# Best Practices
{: .no_toc }

Here are some best practices to consider when building your widgets. For further reading, please refer to the [Developer's Guide](https://github.com/infor-cloud/homepages-widget-sdk/blob/master/DevelopersGuide.pdf).

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Use ION APIs to communicate with the backend
Lorem ipsum

## Use IDS Enterprise component library
Lorem ipsum

## Theme Support
Lorem ipsum

## Translate your widget
Lorem ipsum

## Design for all sizes 
Lorem ipsum

## Add widget screenshots
Lorem ipsum

## Infor Go support
Lorem ipsum

## Build your widgets for the banner area
Lorem ipsum

## Configure a Help URL 
Give your users some help along the way by providing a link to documentation. Use the Help URL property in the widget manifest to add a link to a Support site or documentation. The link will be displayed for end users in the About dialog. 

Configure the link using the `helpUrl` property in the widget manifest. 

### Examples:
```
"helpUrl": "http://www.example.com/" 
"helpUrl": "{Scheme}://{Hostname}:{Port}/{TenantId}/MyApp/Help"
```
