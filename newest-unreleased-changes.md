## 0.11.2
- Added the ability to toggle the usage of JavaScript for both config and per-page frontmadder option. Please note that this will restrict the usage of some shortcodes. To use it you need to turn this on for the specific page you add the shortcodes that require this switch on. Or, you can ignore the `nojs` in log.
- Upgrades Hugo workflow version up to v0.140.2.
- `.LinkTitle` is now used instead of `.Title` for display not in title tag, in case the link title is modified.
- Added ability to add heading ID to documentation pages frontmadder.
- Added SEO HTML tags.
- Added the ability to set image or logo for a specific page that uses listpost partial. See frontmadder configuration variables section.
- Added `linktitle` content variable.
- You can now display last updated time for the entire site. Default is off, and you can turn it on via `display_site_lastmod`. See configuration parameters. On demo page it is turned on.
- Removed details shortcode as it is now built-in.