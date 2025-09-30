+++
keywords = ["doc", "params", "writing", "content", "misc", "title"]
layout = "doc"
title = "Documentation Site"
weight = 1000
+++
# Documentation Site
Hguinav supports built-in documentation template that allows you to create list base documentation pages. Each section, starting at content/, you can create a subsection documentation. You can also look the docs folder of this theme demo.

**Note**: documentation uses both Weight and Title sort styles by default. Please note that when using weight, you also need to set for subsections. Remember that Hugo does not support sorting for specific section? As such, a custom [sort partial]({{% relref "partials/sort.md" %}}) is the actual work implemented in Hguinav to bypass this.

## Setup
First, create the documentation section in content folder, and add _index.md to it containing the following frontmatter. For this documentation, we will create docs folder and use TOML for frontmatter as this theme is TOML based.
```toml
+++
title = "Your Documentation Main Section's Title"
layout = "doc"
+++
Further content for the main documentation section goes here
```

Now, you can create pages with md extention in your documentation folder. Any page within the first section (docs) in this case, is a part of the first section.

You can write documentation as you normally would do, for example:
```toml
+++
title = "Page1"
weight = 1
layout = "doc"
+++
Hello!
```

Note that you also need to set `layout` to `doc` on every page.

## Sections
You can also have subsections inside the main one.

Lets create a subfolder name test inside the main documentation section (docs) in this case.

In the test folder, we will add _index.md with the following content.
```toml
+++
title = "Testing"
layout = "doc"
weight = 1
+++
```

We set weight to 1 because we want to display test section first after main documentation section.

After that, you can write a short description related to that subsection. Do not write long texts in this file, because this will display at the top of the list containing pages related to this section.
```toml
+++
title = "Testing"
layout = "doc"
weight = 1
+++
I am a test section, so you know displaying in first.
```

You may then create pages in the test section usually as pages in the main documentation section.

All content below the frontmatter are done by the [content partial]({{% relref "partials/content.md" %}}) which as support for [variable replacements]({{% relref "writing.md" %}}).

## Frontmatter
The following is a list of params parameters that you can set to documentation section. These parameters are only to be set at the very first section (docs) in this case.

### `label`
An object of labels, i.e. `label.var`.
- `pages`: The label of the pages, default is "Pages".
- `sections`: The label of the sections, default is "Sections".
