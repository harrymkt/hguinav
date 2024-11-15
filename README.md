# UI Navigation
UI Navigation, or known as hguinav, is a Hugo theme designed for accessibility rather than visual and made as easy as possible. Since I am a blind developer, I'd like to develop with accessibility as possible so visually impaired users can use them.

[Theme demo](https://harrymkt.github.io/hguinav)

## License
This theme is distributed under the terms of the [MIT License](https://github.com/harrymkt/hguinav/blob/main/LICENSE.md).

## Features
* Multilingual.
* Customizable extrahead, extrafooter, head, header, footer, with partials, and extrahead, with blocks.
* Documentation site; build accessible documentation sites by using built-in template specifically designed for documentation. You can set the type of the section you want to document in the section's frontmadder.
* Content variables during build, such as `$title$`. See the demo page for documentation
* Copy code blocks; add code blocks which can then be copied using buttons and display the code language if available, helped by JavaScript.
* Local date display; display dates in user's local timezone, no madder what timezone the date is set.

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
* Use 2 level space indentation for HTML. Use 1 tab level indentation for CSS and JavaScript. If Markdown files need indentation, use 1 tab.
* Be the templates accessible for visually impaired and/or blind and prefer readability. Don't worry, I will process in case accessibility issues before pull requests are merged.
* Photos are not required in this theme. You may design with CSS for visual if you so wish.

Thank you!