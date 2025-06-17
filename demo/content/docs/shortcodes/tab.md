+++
keywords = ['doc', 'content', 'shortcode', 'tab']
layout = 'doc'
title = 'Tab Shortcode'
+++
# Tab Shortcode
This shortcode allows you to create a tab panel. It is to be used with the `tabcontent` shortcode.
These shortcodes require the JavaScript usage to be enabled.

## Tab Shortcode (tab.html)
Always use `<` and `>` signs for this shortcode.
- `name`(string) required: The name of the tab.
- `id`(string) required: The identifier of the tab.

## Tab Content Shortcode(tabcontent.html)
Always use `%` sign for this shortcode.
- `id`(string) required: The identifier of the tab that is previously defined.
- `visible`(bool) optional: Toggles whether this tab should display as soon as the tab content is defined.

## Example
```markdown
{{</* tab name="Tab 1" id="1" */>}}
{{</* tab name="Tab 2" id="2" */>}}
{{</* tab name="Tab 3" id="3" */>}}

{{%/* tabcontent id="1" visible=true */%}}
## Content for Tab 1
This is the content for the first tab.
{{%/* /tabcontent */%}}
{{%/* tabcontent id="2" */%}}
## Content for Tab 2
This is the content for the second tab.
{{%/* /tabcontent */%}}
{{%/* tabcontent id="3" */%}}
## Content for Tab 3
This is the content for the third tab.
{{%/* /tabcontent */%}}