---
layout: page
title: Formatting with Jekyll
description: Formatting and Text Editing in Jekyll
order: 2
---

# {{ page.title }}

| parameter | description |
|-----------|-------------|
| `file`    | path to example file for embedding (must be rooted in `_includes`) |
| `syntax`  | (optional) hint for syntax hilighter; defaults to file extension |
| `id_only` | (optional) when `'true'` (string value), macro only evaluates to id of example label, e.g. to use in an href; defaults to empty string and normal behavior of embedding code example |
{:.ui.celled.table}

#### markdown
{:.ui.attached.tertiary.inverted.tight.grey.segment}

<div>
    {% raw %}{% include collapsible_example.liquid file='snippets/hello_world.cpp' %}{% endraw %}
</div>
{:.ui.attached.secondary.tight.segment}

<br>

#### result
{:.ui.attached.secondary.inverted.tight.blue.segment}

{::options parse_block_html="false" /}
<div>
{% include collapsible_example.liquid file='snippets/hello_world.cpp' %}
</div>
{:.ui.attached.secondary.segment}
{::options parse_block_html="true" /}