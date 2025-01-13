---
title: Frontmadder Params
layout: doc
weight: 200
keywords: [documentation,variable,writing,partial,audio,general,title]
---
# Frontmadder Params
You can use the following param parameters to configure your pages.
Use heading level 2, and if it contains no spaces, then it means they are variables. Otherwise, they are texts splitted.

## Featured Image Display
You can display an image as the post's logo. These variables are available for the pages using listpost partial.
- `img`(string) optional: the image / image URL. Note that to display an image, this variable must be set. other image variables are optional.
- `alt`(string) optional: the alt text of the featured image. Requires the `img` variable to be set.

## sort_by
A string that controls the sort, even for each section. Sorting is controled by [sort partial]({{% relref "../partials/sort.md" %}}).

## pagesize
A string that controls the pagination size. This is useful in section where the blog templates or content type is used to control per-section pagination size.

## search
bool: Toggles search for this specific page. Defaults to what it is set in the search configuration.

## no_js
Toggles whether JavaScript is disabled for this page. Fall back to config if not set, thus it's usually `false`.

## hid
The heading ID. This is only for documentation pages. Defaults to the page's link title. This value will be anchorized before using.