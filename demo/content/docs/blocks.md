+++
keywords = ["documentation", "title", "writing", "shortcode", "misc", "blocks"]
layout = "doc"
title = "Blocks"
weight = 300
+++
# Blocks
Sometimes partial files are not enough. Or will they be cluttered? Blocks come in. You can define blocks to display content in position the block is defined in the base template. Here are available blocks that you can use to customize further:
- `title`: The title block. This should be completely optional anyway. For example you can use this block combined with [title partial]({{% relref "partials/title.md" %}}) to ease the management of the page title which asumes the site title should be appended after it.
- `beforeheader`: Content before header, or another word, content immediately following the body tag.
- `extraheader`: Content after the header defined in header.html (partial).
- `main`: The main content.
- `extrafooter`: Content close to body end. Usually empty.