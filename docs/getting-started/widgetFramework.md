---
title: Widget Framework2
parent: Getting Started
nav_order: 2
---

# Widget Framework

The framework is responsible for the creation, layout and lifecycle management of all widgets. It owns parts of what an end user would consider to be the widget, including the widget border, widget title bar and widget menu. A widget implementation is not allowed to directly access these parts of the widget. It owns the widget body area, which is the area inside the widget border and below the widget title bar.

## Widget Types
<b> Inline widget (recommended) </b> 
<br> Widget content is loaded in an element that is part of the Homepage DOM.

<b> External widget </b> 
<br> Widget content is loaded in an IFrame with a URL.

<b> Inline hybrid widget </b>
<br>The widget creates an IFrame to load some of its content.

## Widget Implementation Components

<b> Manifest file </b>
<ul>
  <li> Mandatory for all widget types
	<li> Used to define a widget, each widget must have a manifest with all mandatory properties set
	<li> Manifest data is used to create an inline widget or address an external widget
	<li> Contains the information about the widget that is displayed in the widget catalog, and localization. Optional settings metadata
</ul>
  
<b> Script file </b> 
<ul>	
  <li> Mandatory for inline widgets only
	<li> Should be minimized and combined into one file
</ul>

<b> HTML template(s) </b>
<ul>	
  <li> Optional but only applicable for inline and inline hybrid widgets
	<li> For AngularJS, the templates should be inline and registered directly to the template cache
</ul>

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
