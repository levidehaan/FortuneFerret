__Tldr; This website uses git as its cms, it's awesome, give me cookies__

Also this article is just a placeholder, a test item if you will.

---------
## How it's built

One of the cool things about this site is it is built using [Angular.js](http://angularjs.org) which is an amazing framework.<br>
I have been using it for many of my own projects for the front end.<br>
On the backend I use [node.js](http://nodejs.com) and a couple nifty tools in node.<br>
My current favorite is the fork functionality to run multi-core.<br>
I recently updated the site and got some huge performance gains.

So how does this article get loaded?

First the system connects to github and requests my base data if it doesn't have it yet.

So I created a server that would be the middle man between the client and github to pull my files and load them into the site after translating from markdown to html.
( I'm writing this on my tablet and will commit to update my files )

Once the client has connected the server asks github for a list of files in a specific repository (FortuneFerret).

The file name is actually the title of the article (this makes writing concise titles important) for example this article's name is:

HowLevidehaan.comIsBuilt.md it inserts a space after each capital letter.

This allows me to update my pages easily, get comments on articles in github, and get pull requests on articles.

Once the file has been loaded into the users browser then the markdown conversion script runs to render the data nicely.

------------

## More Info

Please feel free to read the code, you will learn so much more.
