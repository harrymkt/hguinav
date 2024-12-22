---
title: "Search"
weight: 2000
keywords: [search,params,variable,writing,partial,general,audio,tab,content,language]
layout: doc
---
# Search
Hguinav has search built-in. This is a quick overview on how to create your search.

## Configuration
These configurations apply on `params` object of the config. See [search configuration]({{% relref "params/config.md#search" %}}).

## Search Formats{#sformats}
### lunr
This uses JSON file to produce the search content and thus slower and not available for very large content.

{{% details summary="Setup details for lunr format" %}}
#### Setup for search page generation (only for lunr format)
First, remember the following:
- search.js is the JS script that helps determine the search results and inputs.
- layouts/_default/search.html is the actual section that will be generated as the search page.
- layouts/_default/search.json is the JSON file containing the site's pages and content for search.
- Search indexes are generated only the titles and keywords. If someone could fix generating a large set of content, then the content can be generated.

Create a folder called `search` in the content directory, and add `_index.md` with the following content:
```md
---
title: Search
outputs:
- html
- rss
- json
---
```

You can also remove the RSS if you don't want to generate RSS for this section, which is usually not needed for RSS to be generated.

You can create the same search for other languages with the `_index.languageCode.md` prefix.
{{% /details %}}

### pagefind
This format is default used in this theme, and is best for large content. However, this cannot be used in preview, such as `hugo serve`. This format requires to have Python installed, and `pagefind[extended]` package.

{{% details summary="Setup Pagefind" %}}
#### Setup Pagefind
Do the following to get up and run Pagefind. We'll asume you have Python installed:
1. Install Pagefind extended version. You can do this by this command up to the root of this repository. `pip install -r requirements.txt`
2. Set the search format in the `searching` object.
3. Build the site. `zola build`
4. Generate the search index. Make sure to replace outputdir with the directory where your built files live. `python -m pagefind --site outputdir`
- Make sure to add `html` tag with the `lang` attribute set if you are building multilingual search.
- If you want to define where to start searching from, add `data-pagefind` to a tag like div.

That's it!
{{% /details %}}