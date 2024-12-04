{{- $summary := "" }}
{{- with .Get "summary" }}
{{- $summary = . }}
{{- else }}
{{- errorf "The %q shortcode requires summary parameter, %q" .Name .Position }}
{{- end }}
{{- $open := false }}
{{- with .Get "open" }}
{{- $open = . }}
{{- end -}}
<details{{ if eq $open true }} open{{ end }}>
<summary>{{ $summary }}</summary>

{{ .Inner }}

</details>