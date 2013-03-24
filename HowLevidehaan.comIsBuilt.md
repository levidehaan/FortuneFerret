**short story: This website uses git as part of a cms**


One of the cool things about this site is it is built using [Angular.js](http://angularjs.org) which is an amazing framework.
<br>
<br>
The first thing I had to do was talk to the github api.
So I created a server that would be the middle man between the client and github to pull my files.
I wrote this middleware layer in [Node.js](http://nodejs.org).
<br>
<br>
Once the client has connected to levidehaan.com the server asks github for a list of files in a specific repository.
<br>
<br>
The file name is actually the title of the article (this makes writing concise titles important) for example this article's name is:
HowLevidehaan.comIsBuilt.md
<br>
Once the file has been loaded into the users browser then I use a markdown conversion script to render the data in all its proper glory.
<br>
I'll be posting an article on the code of how this works at some point so you don't have to go reading the code to figure out the site, although it is a small amount of code (thanks Angular) so it won't be hard to follow along with.