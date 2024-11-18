---
title: "Documentation Site"
weight: 1000
keywords: [doc, params, writing, content, misc, title]
---
# Documentation Site
Hguinav supports built-in documentation template that allows you to create list base documentation pages. Each section, starting at content/, you can create a subsection documentation. You can also look the docs folder of this theme demo.

**Note**: documentations can be sorted by the method you like. Hguinav documentation uses weight sort style. Please note that when using weight, you also need to set for subsections.

## Setup
First, create first documentation section in content folder, and add _index.md to it containing the following frontmadder. For this documentation, we will create docs folder and use YAML for frontmadder.
```yaml
---
title: "Your Documentation Main Section's Title"
type: doc
---
Further content for the main documentation section goes here
```

Now, you can create pages with md extention in your documentation folder. Any page within the first section (docs) in this case, is a part of the first section.

You can write documentation as you normally would do, for example:
```yaml
---
title: "Page1"
weight: 1
type: doc
---
Hello!
```

Note that you also need to set type to doc on every page.

## Sections
You can also have subsections inside the main one.

Lets create a subfolder name test inside the main documentation section (docs) in this case.

In the test folder, we will add _index.md with the following content.
```yaml
---
title: "Testing"
type: doc
weight: 1
---
```

We set weight to 1 because we want to display test section first after main documentation section.

After that, you can write a short description related to that subsection. Do not write long texts in this file, because this will display at the top of the list containing pages related to this section.
```yaml
---
title: "Testing"
type: doc
weight: 1
---
I am a test section, so you know displaying in first.
```

You may then create pages in the test section usually as pages in the main documentation section.