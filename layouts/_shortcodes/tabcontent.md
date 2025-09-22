{{- $visible := false }}
{{- with .Get "visible" }}
	{{- $visible = . }}
{{- end }}
{{- $nojs := .Page.Site.Params.no_js | default false }}
{{- with .Page.Params.no_js }}
	{{- $nojs = . }}
{{- end }}
{{- if eq $nojs true }}
	{{- erroridf "nojs" "The shortcode name %s cannot be used when JavaScript usage is disabled. %s" .Name .Position }}
{{- end -}}
<div class="tab-content" id="tab-content-{{ .Get "id" }}" style="display: none;">

{{ partial "content.html" (dict "page" .Page "value" .Inner) | safeHTML }}

</div>{{ if (eq $visible true) }}<script>switch_tab("{{ .Get "id" }}");</script>{{ end }}
