{{- $visible := false }}
{{- with .Get "visible" }}
{{- $visible = . }}
{{- end -}}
<div class="tab-content" id="tab-content-{{ .Get "id" }}" style="display: none;">

{{ partial "content.html" (dict "page" .Page "value" .Inner) | safeHTML }}

</div>{{ if (eq $visible true) }}<script>switch_tab("{{ .Get "id" }}");</script>{{ end }}