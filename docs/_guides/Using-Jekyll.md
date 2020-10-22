---
layout: page
title: Using Jeykll
description: Basic Jekyll How-Tos
order: 1
---

# {{ page.title }}


Jekyll is a static site generator written in Ruby.  You'll need to download it with RubyGems in order to edit/preview any docs hosted here.

After you clone the Github repo, install the Jekyll gem:

`sudo gem install jekyll bundler`


Once you've made changes you want to preview, run the serve command to locally host the site:

`bundle exec jekyll serve`

Running that command should output the address where you're hosting the site locally, so open your browser and type in the address like:

`localhost:4000` (or whatever the address is).  Refresh and voila.

To render any drafts in the draft folder, add the --draft flag:

`jekyll serve --draft`


 You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](https://jekyllrb.com/)