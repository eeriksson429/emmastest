---
title: Designing widgets
parent: Documentation
nav_order: 4
---

# Designing widgets

Widgets should use [Enterprise Components for Infor Design System](https://design.infor.com/code/ids-enterprise/latest) or follow Infor design guidelines. 

## Enterprise Components for Infor Design System

[Enterprise Components for Infor Design System](https://design.infor.com/code/ids-enterprise/latest) is a framework-independent UI component library built in js and css that is pattern-focused, template-driven, touch-enabled, responsive, accessible, and themable.

We recommend that you use the IDS Enterprise Components for the UI. Only minimal custom styling should be used, such as altering margins or paddings. 

### Avoid custom components

Complex custom components should always be avoided. 

If custom styling or components has been used, they must follow the IDS guidelines for look & feel, theming, mobile and accessibility support.

## Theme Support

Homepages may run in three different themes variants of the [IDS Subtle Theme](https://design.infor.com/code/ids-enterprise/latest/personalize#themes); Dark, Light and High Contrast. Widgets must support all these themes.

If custom styles have been used, then those styles must work for all three themes. The styles should not be duplicated based on theme but should be written in such a way that only the difference between the themes are extracted into its own style. 

### Running different themes in the Development Container
To run the development container in the different themes the index.html file needs to be changed to include the different style sheets. Note that it is the lime stylesheet as well as xi stylesheet that needs to be changed. Uncomment the stylesheets that you would like to use for the moment and refresh.
