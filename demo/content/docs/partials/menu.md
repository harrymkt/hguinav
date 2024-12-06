---
title: Menu Partial
layout: doc
keywords: [documentation,menu]
---
# Menu Partial (menu.html)
Use this partial to display menus.
- `page`(object) required: The object pointing to the page you want to process, specifically the current page.
- `menuID`(string) required: The menu to process.
- `format`(string) optional: The format you want to use. Using an invalid format will fail the build. Valid formats are:
	- `default`: Default format, with heading and navigation tag.
	- `noheading`: No heading format, only list. This is useful for other menus such as footer.