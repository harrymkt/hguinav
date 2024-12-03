{{- $visible := false }}
{{- with .Get "visible" }}
{{- $visible = . }}
{{- end -}}
<div class="tab-content" id="tab-content-{{ .Get "id" }}" style="display: none;">

{{ .Inner }}

</div>{{ if (eq $visible true) }}<script>switch_tab("{{ .Get "id" }}");</script>{{ end }}