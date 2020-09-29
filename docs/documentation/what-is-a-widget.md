---
title: What is a widget
parent: Documentation
nav_order: 2
---

# What is a widget?
A widget can be defined as a small, single-purpose application that provides quick, at-a-glance information or quick access to simple interactive functions. Widgets are simpler and faster to access than full applications (apps) that may provide more functionality.

Homepages may contain one or many pages and each page may contain one or many widgets. Widgets can be added to a page from the Widget Catalog.

# Widget Framework

The widget framework is responsible for the creation, layout and lifecycle management of all widgets. It owns parts of what an end user would consider to be the widget, including the widget border, widget title bar and widget menu. A widget implementation is not allowed to directly access these parts of the widget. It owns the widget body area, which is the area inside the widget border and below the widget title bar.



## Inline Widget API
An inline widget AMD module must expose a widget factory function, IWidgetInstance widgetFactory(context: IWidgetContext). This function will be called by the framework when the widget is created.

<b>IWidgetContext</b>
<ul>
  <li>Represents the runtime context for a widget
  <li>Settings, widget data, DOM element, framework API etc.  
  <li>Specific for each widget instance  
</ul>

<b>IWidgetInstance</b>
<ul>
  <li>Represents a widget instance
  <li>Optional functions called by the framework to notify the widget of state changes, settings updated etc.
  <li>Defines widget actions, which will appear in the widget menu, and as a button next to the menu if set to primary  
</ul>
