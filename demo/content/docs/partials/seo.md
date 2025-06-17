+++
keywords = ['variable', 'seo', 'content', 'doc', 'params']
layout = 'doc'
title = 'SEO Partial'
+++
# SEO Partial (seo.html)
Use this partial to generate SEO tags specified by its format. If you only pass one value, use the dot(`.`) to pass the current page.
- `page`(page) required: The current page.
- `formats`(slice/string): A slice or a string specifying the [formats](#formats) you wish to generate for. If not set, all formats will be generated.

## Available formats{#formats}
These are located in seos directory.
- `opengraph`: Open Graph.
- `schema`: Schema.