---
title: "Search"
weight: 2000
keywords: [search,params,variable,writing,partial,general,audio,tab,content,language]
layout: doc
---
# Search
Hguinav has search built-in. This is a quick overview on how to create your search.

First, remember the following:
- search.js is the JS script that helps determine the search results and inputs.
- layouts/_default/search.html is the actual section that will be generated as the search page.
- layouts/_default/search.json is the JSON file containing the site's pages and content for search.
- Search indexes are generated only the titles and keywords. If someone could fix generating a large set of content, then the content can be generated.

Once you have above notes you can now start creating your search feature.

## Step 1 (setup for search page generation)
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

## Step 2 (generate the site)
Build or serve your site, and navigate to /search.

You will now see the search input, with results underneeth it.