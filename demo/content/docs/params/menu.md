+++
keywords = ['menu', 'variable', 'config', 'params', 'frontmadder', 'general', 'partial']
layout = 'doc'
title = 'Menu Params'
weight = 300
+++
# Menu Params
You can use the following param parameters to configure your menus. These variables should be put under the `params` object of the menu.

## attributes
Specify the custom attributes you want to add. These attributes will be placed before the `href` of the link element (the `a` tag).

example:
```yaml
menus:
  main:
    - name: test
      pageRef: /
      params:
        attributes:
          class: "active"
```