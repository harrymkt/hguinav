+++
keywords = ['variable', 'config', 'content', 'writing']
layout = 'doc'
title = 'Title Partial'
+++
# Title Partial (title.html)
You can use this partial to customize the title of any page. Use the `title` block to customize.

You can pass one parameter (a slice of titles) if you only want one parameter. Otherwise, use `dict` to provide more parameters.
- `titles`(slice): The titles made out of slice.
- `sep`(string) optional: The title's separator. Defaults to what it is set in `title_sep` site param.
- `overwrite`(bool) optional: `false` if the site title should be appended after the titles, or `true` otherwise. Defaults to `false`.

## Example
```go-html-template
{{- define "title" -}}
{{ $titles := slice .Title -}}
{{- if and .Paginator (gt .Paginator.PageNumber 1) -}}
{{- $titles = $titles | append (printf " (page %v)" .Paginator.PageNumber) -}}
{{- end -}}
{{- partial "title.html" (dict "titles" $titles) -}}
{{- end -}}
```