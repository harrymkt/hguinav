# UI Navigation
UI Navigation, or known as hguinav, is a Hugo theme designed for accessibility rather than visual and made as easy as possible. Since I am a blind developer, I'd like to develop with accessibility as possible so visually impaired users can use them.

This theme is also available for Zola at [Zluinav](https://github.com/harrymkt/zluinav).

This theme uses blocks as possible because as far as I know Hugo does not allow extend and super functions like other static site generators.

[Theme demo](https://harrymkt.github.io/hguinav)

## License
This theme is distributed under the terms of the [MIT License](https://github.com/harrymkt/hguinav/blob/main/LICENSE.md).

## Features
- Multilingual support with i18n; Hugo supports built-in advance multilingual feature, this theme only adds templates for it.
- Customizable extrahead, extrafooter, head, header, footer, with partials, and extrahead, with blocks.
- Documentation site; build accessible documentation sites by using built-in template specifically designed for documentation. You set the layout of the section you want to document as well as in each page of that related document.
- Content variables during build, such as `%title%`. See the demo page for documentation
- Sort pages by the way you like and for specific sections, which is by default not supported. This uses the sort partial.
- Define menu pages that check for multilingual with the special menu partial.
- Copy code blocks; add code blocks which can then be copied using buttons and display the code language if available, helped by JavaScript.
- Local date display; display dates in user's local timezone, no madder what timezone the date is set.
- Taxonomies support.
- Taxonomy based author / user management, provided in demo.
- Use blocks to easily modify without having to copy some files to your layouts.
- Use partials and shortcodes to make your content and/or templates shorten.
- Comprehensive documentation; Hguinav provides a full Comprehensive documentation including possible layouts, templates, shortcodes, blocks, configurable parameters, and more, everything as it updates.

## Installation
Using git:
```bash
cd themes
git clone https://github.com/harrymkt/hguinav.git
```
Or [download manually](https://github.com/harrymkt/hguinav/archive/refs/heads/main.zip) and paste in the themes directory.

Or, add to the Git submodule
```bash
git submodule add --name hguinav https://github.com/harrymkt/hguinav.git themes/hguinav
git submodule update --remote
```

Next, set the theme in your config.

## Configuration
Please read the [documentation](https://harrymkt.github.io/hguinav) for more information and configuration options.

## Contribution
Contributions to this theme are welcome, provided that the following requirements are met:
- Use 2 level space indentation for HTML. Use 1 tab level indentation for CSS and JavaScript. If Markdown files need indentation, use 1 tab.
- Be the templates accessible for visually impaired and/or blind and prefer readability. Don't worry, I will process in case accessibility issues before pull requests are merged.
- Photos are not required in this theme. You may design with CSS for visual if you so wish.

Thank you!