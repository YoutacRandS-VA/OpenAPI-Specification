---
owner: mikekistler
issue:
description: structured fields boolean as defined in [RFC8941]
source: https://www.rfc-editor.org/rfc/rfc8941#name-booleans
source_label: RFC 8941
base_type: string
layout: default
---

# <a href="..">{{ page.collection }}</a>

## {{ page.slug }} - {{ page.description }}

Base type: `{{ page.base_type }}`.

The `{{page.slug}}` format represents a structured fields boolean as defined in [RFC8941].

```abnf
sf-boolean = "?" boolean
boolean    = "0" / "1"
```

A Boolean is indicated with a leading "?" character followed by a "1" for a true value or "0" for false.

This format is appropriate for a header value that must conform to the {{page.slug}} structured field definition.

{% if page.issue %}
### GitHub Issue

* [#{{ page.issue }}](https://github.com/OAI/OpenAPI-Specification/issues/{{ page.issue }})
{% endif %}

{% if page.remarks %}
### Remarks

{{ page.remarks }}
{% endif %}

[RFC8941]: https://www.rfc-editor.org/rfc/rfc8941#name-booleans