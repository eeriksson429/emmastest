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
You can add up to three PNG image files that will be shown when viewing the widget in the Widget Catalog. The screenshots helps communicate the widget's features and visual experience for your end users. 

![Screenshot of Widget Catalog](../assets/images/widget-catalog_screenshots-example.png)

Configure your screenshots by adding up to three PNG image files in the widget ZIP. The screenshots must be named `screenshot1.png` `screenshot2.png` etc. The image will be displayed in a 200x200px container, and if the image is clicked the image is shown in its original size.

Reference the images using the `screenshots` property in the widget manifest. The value should reflect the number of screenshots. 

### Example:
{: .no_toc }
```
"screenshots": "2" 
```

## Infor Go support
Lorem ipsum

## Build your widgets for the banner area



## Configure a Help URL 
Give your users some help along the way by providing a link to documentation. The link will be displayed for end users in the About dialog. 

Configure the link by adding the `helpUrl` property in the widget manifest. 

### Examples:
{: .no_toc }
```
"helpUrl": "http://www.example.com/" 
"helpUrl": "{Scheme}://{Hostname}:{Port}/{TenantId}/MyApp/Help"
```
