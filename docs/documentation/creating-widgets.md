---
title: Creating widgets
parent: Documentation
nav_order: 3
---

# Creating widgets 

## Widget Types

There are three types of widgets; inline, external and inline hybrid.

| Widget Type | Description |
| ------------- | ------------- |
| Inline (recommended) | Widget content is loaded in an element that is part of the Homepage DOM. |
| External | Widget content is loaded in an IFrame with a URL  |
| Inline hybrid | The widget creates an IFrame to load some of its content. |

We recommended that you use the inline widget type when creating your widgets. 

## Widget Technology Choice

For widgets with simple functionality and hybrids with for example a custom settings UI, we recommend using jQuery.

For complex widgets Angular and TypeScript is a better fit. If Angular is the selected framework, we recommend that you use it with TypeScript.

## Widget Components

| Component | Description |
| ------------- | ------------- |
| Manifest file | Mandatory for all widget types. Used to define a widget, each widget must have a manifest with all mandatory properties set.  Manifest data is used to create an inline widget or address an external widget. Contains the information about the widget that is displayed in the widget catalog, and localization. Optional settings metadata  |
| Script file | Mandatory for inline widgets only. Should be minimized and combined into one file | 
| HTML template(s) | Optional but only applicable for inline and inline hybrid widgets. |

## Widget Manifest

The widget manifest is used to define a widget and each widget must have a manifest with all mandatory properties set. 

Below is a list of the mandatory properties. For optional properties, please refer to the [Developer's Guide](https://github.com/infor-cloud/homepages-widget-sdk/blob/master/DevelopersGuide.pdf).

### Widget ID
The unique widget identifier. The ID must be unique among all widgets and should be chosen carefully. 
```
"widgetId": "infor.sample.helloworld"
```
```
"widgetId": "infor.mingle.actions"
```

### Type
The type of widget. The only supported types are inline and external. A hybrid widget should be defined as inline.
```
"type": "inline"
```

### Version
The widget version number. The version number should consist of a minimum of two and a maximum of four positive integers separated by dots.
```
"version": "1.0.0.0"
```

### Name
The name of the widget. This name will never be visible for an end user and is mainly intended administration purposes.
```
"name": "Hello World"
```

## Title & Description vs Localization
Either Title and Description OR a Localization block with "en-US" and "widgetTitle" and "widgetDescription" is mandatory.

### Module Name
The name of the widget AMD module used to load the widget with SystemJS. This property is only mandatory if the widget type is inline.
```
"moduleName": "widget"
```

### URL
The URL or URL template for an external widget. This property is only mandatory if the widget type is external. 
```
"url": "https://server/path"
```
```
"url": "{scheme}://{hostname}:{port}/{context}"
```

### Framework
The client framework that the widget is using. Valid values are "angular" or "jquery". This property is only mandatory if the widget type is inline.
```
"framework": "angular"
```

### Author
The author of the widget. Note that this is only required for Tenant Widgets. 
```
"author": "Sample Corporation"
```
