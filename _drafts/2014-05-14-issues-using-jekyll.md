When I first started using [Jekyll](http://jekyllrb.com) to create this blog I didn't really run into any problems.  It was only when I decided to deploy it to (Github Pages)[http://pages.github.com] that I ran into problems.  Turns out that the library that Jekyll ships with by default to compile `markdown` is old and not maintained anymore.  It was an easy fix.  Just had to add this to my `_config.yml` file:

~~~ yml
markdown: kramdown

~~~

Github notified me of this issue via email which made it easy to diganose and fix.  The second issue that I ran into was when using `haml` for the `index` page.  It appears that even with the haml plugin installed for Jekyll Github didn't want to display it.  As soon as I changed the index file back to `index.html` Github Pages picked up the blog and started to display it.
