+++
keywords = ['frontmatter', 'sort', 'blocks', 'params', 'paginate']
layout = 'doc'
title = 'Paginate Partial'
+++
# Paginate Partial (paginate.html)
Paginates a given section as context. It can be one value (the page), or you can specify more than one by using `dict`. The pagination size will be determined by the page you give. See [frontmatter variables]({{% relref "../params/frontmatter.md" %}}).

The following parameters are available:
- `page`(page) required: The page object, usually the current page.
- `sort_by`(string) optional: The sorting method. See [sort partial]({{% relref "sort.md" %}}). Defaults to none.
- `reverse`(bool) optional: Should the pages be reversed? Useful if you sort by `Date`, `Lastmod`, etc. Defaults to `false`.