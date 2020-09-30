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

## Style sheet classes
There are a few Homepages framework classes that can be used by widget developers. These are used when the standard Infor Design System classes are not enough.

| Name | Light | Dark | High Contrast | Notes |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| lm-bg | #f0f0f0 | #313236 | #d8d8d8 | Used for layout backgrounds, such as the body background. |
| lm-item-bg | #fff | #414247 | #f0f0f0 | Used for item backgrounds, such as widgets or cards. |
| lm-hdr-bg | #d8d8d8 | #50535a | #bdbdbd | Used for headers, such as the catalog header. |
| lm-brd | #bdbdbd | #656871 | #5c5c5c | Used for borders. |
| lm-brd-accent | #d8d8d8 | #212224 | #5c5c5c | Used for borders. |
| lm-icon | #5c5c5c | #abaeb7 | #292929 | Used for icons. |
| lm-icon-accent | #1a1a1a | #fff | #5c5c5c | Used when hovering icons. |
| lm-fg | #1a1a1a | #fff | #1a1a1a | The default text color. |
| lm-white | #fff | #fff | #fff | Used where text always should be light. |