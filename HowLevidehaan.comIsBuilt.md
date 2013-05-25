__short story: This website uses git as its cms__

## How it's built

One of the cool things about this site is it is built using [Angular.js](http://angularjs.org) which is an amazing framework.

The first thing I had to do was talk to the github api.
So I created a server that would be the middle man between the client and github to pull my files.
I wrote this middleware layer in [Node.js](http://nodejs.org).

Once the client has connected to levidehaan.com the server asks github for a list of files in a specific repository.

The file name is actually the title of the article (this makes writing concise titles important) for example this article's name is:
HowLevidehaan.comIsBuilt.md basically it splits on capitals at the moment.
The reason for this is so I don't have to pull the content until the user clicks the drop down link.

Once the file has been loaded into the users browser then I use a markdown conversion script to render the data in all its proper glory.

###I will probably be switching over to google docs as a document provider instead of github so I don't have to use markdown.

## More Info

I'll be posting an article on the code of how this works at some point so you don't have to go reading the code to figure out the site, although it is a small amount of code (Thanks to Angular) so it won't be hard to follow along with.

