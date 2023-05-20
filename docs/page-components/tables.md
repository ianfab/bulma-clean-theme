---
layout: page
title: Tables
subtitle: Page Components
menubar: docs_menu
show_sidebar: false
toc: true
---

## Table Include

The table modal allows you to render a table from a data file, e.g., CSV or TSV.

The include needs only the data as argument, and an optional caption, as well as an optional key and value for filtering.

Below are examples for the include.

{% raw %}
<code>
{% include table.html data=site.data.example_table caption="example table" %}
</code>

<code>
{% include table.html data=site.data.example_table caption="filtered table" key="b" value="5" %}
</code>
{% endraw %}

## Example Table Include

<div>
{% include table.html data=site.data.example_table caption="example table" %}
</div>

<div>
{% include table.html data=site.data.example_table caption="filtered table" key="b" value="5" %}
</div>
