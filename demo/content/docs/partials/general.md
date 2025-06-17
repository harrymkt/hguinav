+++
keywords = ['writing', 'config', 'doc', 'params', 'content', 'base', 'related']
layout = 'doc'
title = 'General Partials'
+++
# General Partials
The following are partials that do not necessary to document each page.

## extrafoot.html
Extra footer, such as JS scripts to add to the end of but before closing body.

## extrahead.html
Extra head meta information put before the title block.

## footer.html
Main footer.

## head.html
Main head meta immediately following the head tag. Note: title is only used by title block, which allows you to customize the title from within any section / page using [title partial]({{% relref "title.md" %}}).

## header.html
Header, before navigation.

## listpost.html
Use to list pages in pagination. Add the partial [pagination]({{% relref "pagination.md" %}}) after this partial to add pagination buttons. The pagination.html takes paginator object.

## nav.html
Use to add navigation. This is made to be easy as possible to overwrite since Hugo's templating is restricted.