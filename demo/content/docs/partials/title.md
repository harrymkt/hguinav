---
title: Title Partial
type: doc
weight: 200
keywords: [variable,config,content,writing]
---
# Title Partial (title.html)
You can use this partial to customize the title of any page. The site title will be appended after them. Use the `title` block to customize.
* `titles`(slice): The titles made out of slice.

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