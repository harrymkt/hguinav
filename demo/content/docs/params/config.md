+++
keywords = ['doc', 'documentation', 'variable', 'writing', 'partial']
layout = 'doc'
title = 'Config Params'
weight = 100
+++
# Config Params
You can use the following param parameters to configure the theme in your site config.

## title_sep
The title's seperator to use. Default is " – ".

## no_js
Toggles whether JavaScript is disabled. Defaults to `false`.

## display_site_lastmod
Toggles whether the entire site last updated date should display. Defaults to `false`.

## search
Search configuration options:
- `enable`(bool): Toggles search. Defaults to `true`
- `default_enable`(bool): Default search status. This is useful to turn this off and manually turn on in the frontmadder of the pages you want. Defaults to `true`
- `format`(string): One of the [search formats]({{% relref "../search.md#sformats" %}}). Defaults to `pagefind`