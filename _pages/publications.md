---
permalink: /publications/
title: "Publications"
---

<br />
<a href="/assets/files/moodie_cv.pdf" class="btn btn--primary" target="_blank">A complete CV is available here</a>

## Manuscripts *in preparation* and *in review*

{% bibliography --file group_publications --query @article[ entrysubtype != nopeer && pubstate^=in] --bibliography_list_attributes {:reversed=>'reversed'} %}



## Manuscripts published

<!-- {% bibliography --file group_publications --query @article[ entrysubtype != nopeer && pubstate != inreview && pubstate != inpreparation && pubstate != inrevision] --reverse %} -->

{% bibliography --file group_publications --query @article[ entrysubtype != nopeer && pubstate != inreview && pubstate != inpreparation && pubstate != inrevision && pubstate != inpress && pubstate != submitted] --bibliography_list_attributes {:reversed=>"reversed"} %}
