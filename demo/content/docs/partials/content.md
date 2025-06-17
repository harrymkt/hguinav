+++
keywords = ['variable', 'config', 'content', 'write', 'params']
layout = 'doc'
title = 'Content Partial'
+++
# Content Partial (content.html)
You can use this partial to display content instead of using `{{ .Content }}` etc. The advantage of using this partial is that it allows you to add content variables. See [writing]({{% relref "/docs/writing" %}}) to see how variables work.
- `value`(string) required: The value to display.
- `page`(object) required: The page object where the content partial should retrieve necessary variables to replace.

## Example
```go-html-template
{{ (partial "content.html" (dict "value" .Content "page" . )) | safeHTML }}
```