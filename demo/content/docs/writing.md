+++
keywords = ['content', 'variable', 'writing', 'config']
layout = 'doc'
title = 'Writing'
weight = 200
+++
# Writing
You can use the following variables to replace with something else. Variables are enclosed by `%variable_name%` where variable_name is the name of available variables you want. This feature can be used in content files where the [content partial]({{% relref "partials/content.md" %}}) is used, such as documentation sections, home page, blog, etc.

To display the raw of the variable name itself, prefix with `/`. For example, %//title%

Be warned that failure to retrieve the variable will render that string directly.

## Supported variables:
- `title`: The title of the page.
- `date`: The published date in the local format, similar to post page.
- `updated`: The updated date, similar to above format.
- `description`: The description.
- `linktitle`: The friendly title of the page (`linkTitle` frontmatter). Falls back to title if not set.

## Example
```markdown
+++
title = "Test"
+++
This page is titled %/title%
```
