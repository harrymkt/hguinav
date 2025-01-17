---
title: Sort Partial
layout: doc
keywords: [config,writing,partial,general,content,menu,doc]
---
# Sort Partial (sort.html)
You can use this partial to sort specific sections the way you want. See [frontmadder variables]({{% relref "../params/frontmadder.md" %}}).
- `sorts`(collection) required: The pages collection.
- `sortby`(string) optional: Which way would you like the pages to be sorted? Eg, `Title`, `Weight`, `Date`.
- `reverse`(bool) optional: Should the pages be reversed after sorting? Defaults to `false`. Useful if you are sorting by `date`, `lastmod` etc.

## Example
```go-html-template
{{- $pages := partial "sort.html" (dict "sorts" .RegularPages "sortby" "Title") }}
```