##Replace UTM
A chrome extension that automatically replaces UTM campaign parameters with "The Dark Funnel".  Based on an existing extension by Sitha Milli (https://smithamilli.com/fuck-utm/). 

All I did was change what gets replaced - a constant defined in the javascript - and then install it locally

##Caveats
- The extension checks the "href" attribute of all <a> tags, so it won't work if a url in a link is shortened.
- Because the extension redirects you to links via Javascript in very rare instances if a site uses event handlers in an obfuscated way there is a possibility of something not working.  An example of this has not yet been seen though.
