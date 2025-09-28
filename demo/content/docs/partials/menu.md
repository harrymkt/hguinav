+++
keywords = ['documentation', 'menu']
layout = 'doc'
title = 'Menu Partial'
+++
# Menu Partial (menu.html)
Use this partial to display menus.
- `page`(object) required: The object pointing to the page you want to process, specifically the current page.
- `menuID`(string) required: The menu to process.
- `label`(string): The label of the menu navigation, especially for default format. Default will be the result of `mainmenu` key in i18n translation.
- `format`(string) optional: The format you want to use. Using an invalid format will fail the build. Valid formats are:
	- `default`: Default format, with heading and navigation tag.
	- `noheading`: No heading format, only list. This is useful for other menus such as footer.
