+++
keywords = ['documentation', 'config', 'writing', 'partial', 'related', 'general', 'misc']
layout = 'doc'
title = 'Related Partial'
+++
# Related Partial (related.html)
Use this partial to display related content. You can pass one value (the current page (the dot)), or you can use `dict` to provide one or more values.
- `page`(object) required: The object pointing to the page you want to process, specifically the pages.
- `text`(string) optional: The text to display on heading.
- `hlevel`(int) optional: The level of the heading, default is 4.
- `count`(int) optional: The number of elements to retrieve. Defaults to `5`.