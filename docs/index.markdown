---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Welcome!
category: home
description: overview of DocPOC 
---

# {{ page.title }}

The goal of **DocPOC** is to build a site using [Jekyll] and hosted by [Github Pages] that makes it easy to publish and maintain our documentation.
{:.larger.text}
With Github Pages, the documentation can live inside our existing project repos, so updating it is as simple as opening a PR.

Learn more about using Github Pages and Jekyll in the following guides:
{% include ordered_child_list.liquid docs=site.guides %}

[GitHub Pages]: https://pages.github.com/ "Websites for you and your projects"
[Jekyll]: https://jekyllrb.com/