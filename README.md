##Replace UTM
A chrome extension that automatically replaces UTM campaign parameters with "The Dark Funnel".  Based on an existing extension by Sitha Milli (https://smithamilli.com/fuck-utm/). 

All I did was change what gets replaced - a constant defined in the javascript - and then install it locally

##Caveats
- The extension checks the "href" attribute of all <a> tags, so it won't work if a url in a link is shortened.
- Because the extension redirects you to links via Javascript in very rare instances if a site uses event handlers in an obfuscated way there is a possibility of something not working.  An example of this has not yet been seen though.

##Installing

- Download the zip file and unzip somewhere local that won't get deleted 
- Add a "vendor" directory inside the replace-utm/app/ directory, as a peer to /js/
- Download a version of jquery minified - for example: https://code.jquery.com/jquery-3.7.1.min.js
- Put that in the vendor directory and rename it jquery.min.js
- In chrome, use the three dots (shishkabob) menu to open "manage extensions"
- Make sure "developer mode" is enabled in the upper right
- Choose "load unpacked" and pick the "app" directory of the zip file

If you want to change what the text replacer is, it is defined at line 19 of inject.js 
