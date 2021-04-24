---
layout: default
title: PR {{.Repository.Name}}
parent: {{.Organization.Name}}
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/{{.Organization.Github}}/{{.Repository.Name}}
---

# {{.Repository.Name}}

[Goto GitHub]({{.Repository.Link}}){: .btn .btn-blue }

{{range .PRs}}
<div class="code-example" markdown="1">
| | {{.Title}} |
|:-----|:-----------|
| {{range .Labels}}{{.Name}}{: .label-grey }{{end}} | {{.Body}} |
[View on GitHub]({{.URL}}){: .btn }
</div>
{{end}}