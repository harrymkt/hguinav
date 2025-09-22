# UI Navigation
UI Navigation, or known as hguinav, is a [Hugo](https://gohugo.io/) theme designed for accessibility rather than visual and made as easy as possible. Since I am a blind developer, I would like to develop with accessibility as possible so visually impaired users can use them.

This theme is also available for Zola at [Zluinav](https://github.com/harrymkt/zluinav).

This theme uses blocks as possible because as far as I know Hugo does not allow extend and super functions like other static site generators.

[Theme demo](https://harrymkt.github.io/hguinav)

## License
This theme is distributed under the terms of the [MIT License](https://github.com/harrymkt/hguinav/blob/main/LICENSE.md).

## Features
- Accessibility; Hguinav is designed to be accessible as possible, especially for blind and visually impaired. This is done by using accessibility tags, such as ARIA, and other possible accessibility features.
- SEO friendly.
- Multilingual support with i18n; Hugo supports built-in advance multilingual feature, this theme only adds templates for it.
- Customizable extrahead, extrafooter, head, header, footer, with partials, and extrahead, with blocks.
- Customizable Documentation Site; build accessible [documentation sites](https://harrymkt.github.io/hguinav/docs/documentation) by using built-in template specifically designed for documentation. You set the layout of the section you want to document as well as in each page of that related document.
- [Content variables](https://harrymkt.github.io/hguinav/docs/writing) during build, such as `%title%`.
- Sort pages by the way you like and for specific sections, which is by default not supported. This uses the [sort](https://harrymkt.github.io/hguinav/docs/partials/sort) partial.
- Define per-section pagination size.
- Define menu pages that check for multilingual with the special [menu](https://harrymkt.github.io/hguinav/docs/partials/menu) partial.
- Built-in blog post templates.
- Copy code blocks; add code blocks which can then be copied using buttons and display the code language if available, helped by JavaScript.
- Local date display; display dates in user's local timezone, no matter what timezone the date is set.
- Taxonomies support.
- Taxonomy based [author/user management](https://harrymkt.github.io/hguinav/docs/author-taxonomy), provided in demo.
- Built-in [search](https://harrymkt.github.io/hguinav/docs/search) support, with a variety of search formats.
- Use [blocks](https://harrymkt.github.io/hguinav/docs/blocks) to easily modify without having to copy some files to your layouts.
- Use a large number of partials and shortcodes to make your content and/or templates shorten.
- Ability to toggle the use of JavaScript for both config and per-page frontmadder.
- Comprehensive documentation; Hguinav provides a full Comprehensive documentation including possible layouts, partials, shortcodes, blocks, configurable parameters, and more, everything as it updates.

## Installation
Add to the Git submodule (recommended):
```bash
git submodule add --name hguinav https://github.com/harrymkt/hguinav.git themes/hguinav
git submodule update --remote
```

Or using git clone method:
```bash
cd themes
git clone https://github.com/harrymkt/hguinav.git
```
Or [download manually](https://github.com/harrymkt/hguinav/archive/refs/heads/main.zip) and paste in the themes directory.

Next, set the theme in your config.
`theme = "hguinav"`

## Configuration
Please read the [documentation](https://harrymkt.github.io/hguinav) for more information and configuration options.

## Contribution
Contributions to this theme are welcome, provided that the following requirements are met:
- Use 2 level space indentation for HTML. Use 1 tab level indentation for CSS, TOML and JavaScript. If Markdown files need indentation, use 1 tab.
- Be the templates accessible for visually impaired and/or blind and prefer readability. Don't worry, I will process in case accessibility issues before pull requests are merged.
- Photos are not required in this theme. You may design with CSS for visual if you so wish.
- When creating a pull request it is advised that you:
	- Use different branch other than main; this avoids issues with updating in case your pull request gets rejected.

Thank you!
