---
title: "Author Management Via Taxonomy"
weight: 400
keywords: [documentation,content,partial,author,writing,variable,misc,general,menu]
layout: doc
---
# %title%
You can have taxonomy based author management system. Create each author section in `content/authors/author_name/_index.md`, and looks like this:
```yaml
---
title: "Author name"
role: admin
---
I'm the maintainer of this site (optional byo)
```

Content processing here - is also done by the [content partial]({{% relref "partials/content.md" %}}) which as support for [variable replacements]({{% relref "writing.md" %}}).

Please note that you do not need to create section for that author if you are not adding custom metadata for them.

## Setting Author Taxonomy
In your site configuration:
```yaml
taxonomies:
  author: authors
  # Custom taxonomies go here
```

## Frontmadder
Hguinav provides the following optional frontmadder variables that you can set in your author's page:
- `role`(string): The role of this author, eg admin, for informational purposes.
- `website`(string: Personal website.