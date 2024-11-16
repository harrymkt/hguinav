---
title: Writing
type: doc
weight: 10
keywords: [content,variable,writing,config]
---
# Writing
You can use the following variables to replace with something else. Variables are enclosed by `$variable_name$` where variable_name is the name of available variables you want. This feature can be used in content files where the content partial is used, such as documentation sections, home page, blog, etc.

To display the raw of the variable name itself, prefix with `/`. For example, $//title$

Available variables:
* `title`: The title of the page.

## Example
```markdown
---
title: Test
---
This page is titled $/title$
```