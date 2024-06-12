{%- if include.content -%}
{{ include.label }}: 
{% for item_name in include.content -%}
{%- assign item = include.collection | where: "title", item_name | first -%}
[{{ item.title }}]({% link {{item.path}} %})
{%- if forloop.last -%}{%- else -%}
&nbsp;|&nbsp;
{%- endif -%}
{%- endfor %}
{%- endif -%}