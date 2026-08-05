---
Title: "{{title | escape}}"
Year: {{date | format("YYYY")}}
Authors: {{authors}}
Tags: [{% for t in tags %}{{t.tag}}{% if not loop.last %}, {% endif %}{% endfor %}]
URL: {{url}}
aliases:
  - {{title}}
  - {{citekey}}
---

**Zotero PDF Link:** {{pdfZoteroLink}}
**Relations:** {% for relation in relations | selectattr("citekey") %} [[{{relation.citekey}}]]{% if not loop.last %}, {% endif%} {% endfor %}


> [!INFO] Citation
> {{bibliography}}

> [!abstract] Abstract
> {{abstractNote}}

> [!NOTE]- Persistent Notes
> {% persist "notes" %}{% if isFirstImport %}
> Write notes here!
> {% endif %}
> {% endpersist %}

> [!EXAMPLE]- Annotations
> {% for annotation in annotations -%}
> {%- if annotation.annotatedText -%}
> {% if annotation.color %} <mark class="hltr-{{annotation.colorCategory | lower}}">"{{annotation.annotatedText | safe}}"</mark> {% else %} {{annotation.type | capitalize}} {% endif %}[Page {{annotation.pageLabel}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.pageLabel}}&annotation={{annotation.id}})
> {%- endif %}
> {% if annotation.comment %}
> {{annotation.comment | safe}} [Page {{annotation.pageLabel}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.pageLabel}}&annotation={{annotation.id}})
> {% endif %}
> {%- if annotation.imageRelativePath %} 
> ![[{{annotation.imageRelativePath}}]]
> {%- endif %}
> {% if annotation.allTags %}
> {{annotation.allTags}}
> {% endif %}
> {% endfor -%}

