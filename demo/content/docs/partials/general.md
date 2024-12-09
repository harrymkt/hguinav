---
title: General Partials
layout: doc
keywords: [writing, config, doc, params, content,base,related]
---
# General Partials
The following are partials that do not necessary to document each page.

## extrafoot.html
Extra footer, such as JS scripts to add to the end of but before closing body.

## extrahead.html
Extra head meta information put before the title block.

## footer.html
Main footer.

## head.html
Main head meta immediately following the head tag. Note: title is only used by title block, which allows you to customize the title from within any section / page using [title partial]({{% relref "title.md" %}}).

## header.html
Header, before navigation.

## listpost.html
Use to list pages in pagination. Add the partial pagination.html after this partial to add pagination buttons. The pagination.html takes paginator object.

## nav.html
Use to add navigation. This is made to be easy as possible to overwrite since Hugo's templating is restricted.

## paginate.html
Paginates a given section as context. It can be one value (the page), or you can specify more than one by using `dict`. The pagination size will be determined by the page you give. See [frontmadder variables]({{% relref "../params/frontmadder.md" %}}).

The following parameters are available:
- `page`(page) required: The page object, usually the current page.
- `sort_by`(string) optional: The sorting method. See [sort partial]({{% relref "sort.md" %}}). Defaults to none.
- `reverse`(bool) optional: Should the pages be reversed? Useful if you sort by `Date`, `Lastmod`, etc. Defaults to `false`.