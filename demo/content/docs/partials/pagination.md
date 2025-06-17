+++
keywords = ['sort', 'blocks', 'params', 'paginate', 'paginator']
layout = 'doc'
title = 'Pagination Partial'
+++
# Pagination Partial (pagination.html)
Adds the pagination area. If you pass only one value, then it must be the paginator object result of either `.Paginator` or `.Paginate` method, or by the [paginate partial]({{% relref "paginate.md" %}}). You can also pass multiple parameters.

The following parameters are available:
- `paginator`(pager) required: The pager object.