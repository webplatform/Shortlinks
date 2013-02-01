wpd.mx shortlinks configuration
===============================

This repository contains all explicitly defined shortlinks for the http://wpd.mx domain.

The format of the shortlinks.txt file is very simple: `<key> <space> <value>`.
`<key>` is the short part after the domain
`<space>` is any number of whitespaces
`<value>` is the URL the client is redirected to
Commented lines start with a `#`.

http://wpd.mx itself redirects to the wiki's main page. If something is provided after the slash, it is searched for in the shortlinks.txt file. If a match is found, it is sent as the redirect. If nothing could be found, the client gets redirected to the wiki search, which in turn displays the article (if a valid title was provided) or display the search results for the provided value.

Examples:
* http://wpd.mx -> http://docs.webplatform.org/wiki/Main_Page
* http://wpd.mx/tasks -> http://docs.webplatform.org/wiki/WPD:Most_Wanted_Tasks
* http://wpd.mx/apis/canvas -> http://docs.webplatform.org/wiki/apis/canvas
* http://wpd.mx/gradient -> Search for "gradient"

The master branch is pulled every hour, so changes should be live in under 60 minutes.

If you have questions or comments contact fr0zenice on #webplatform (freenode) or at frozenice@frozenice.de!
