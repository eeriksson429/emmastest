---
title: Packaging and Deployment
parent: Documentation
nav_order: 3
---

# Packaging and Deployment

Concluding text...

## Packaging
### Files to include
A widget package should only include the files that are required in runtime. Any files that are not used in runtime such as source files or build artifacts should be excluded from the widget package. The widget packages are synchronized over networks and stored in databases and should be as small as possible.

#### Mandatory files
Which files are mandatory depends on the widget type.

<br><i> Widget manifest </i>
<br> A widget manifest file called widget.manifest is required for all type of widgets.

<br><i> Widget module file </i>
<br> A widget module file is required for inline widgets. Example: widget.js

#### Optional files
Optional files could be image files.


Eller ska man bara hänvisa till guiden för packaging?
