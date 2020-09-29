---
title: Introduction
parent: Documentation
nav_order: 2
---

# Introduction

The Widget SDK is used to build widgets for [Infor Homepages](https://www.youtube.com/watch?v=PP7f6T442JY).

## What is a widget?
A widget can be defined as a small, single-purpose application that provides quick, at-a-glance information or quick access to simple interactive functions. Widgets are simpler and faster to access than full applications (apps) that may provide more functionality.

Homepages may contain one or many pages and each page may contain one or many widgets. Widgets can be added to a page from the Widget Catalog.

## Widget Types

There are three types of widgets; inline, external and inline hybrid.

| Widget Type | Description |
| ------------- | ------------- |
| Inline (recommended) | Widget content is loaded in an element that is part of the Homepage DOM. |
| External | Widget content is loaded in an IFrame with a URL  |
| Inline hybrid | The widget creates an IFrame to load some of its content. |


## Widget Components

| Component | Description |
| ------------- | ------------- |
| Manifest file | Mandatory for all widget types. Used to define a widget, each widget must have a manifest with all mandatory properties set.  Manifest data is used to create an inline widget or address an external widget. Contains the information about the widget that is displayed in the widget catalog, and localization. Optional settings metadata  |
| Script file | Mandatory for inline widgets only. Should be minimized and combined into one file | 
| HTML template(s) | Optional but only applicable for inline and inline hybrid widgets. |