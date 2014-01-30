__Tldr; This website uses git as its cms, it's awesome, give me cookies__

Also this article is just a placeholder, a test item if you will.

---------
## How it's built

One of the cool things about this site is it is built using [Angular.js](http://angularjs.org) which is an amazing framework.

I have been using it for many of my own projects for the front end. On the backend I use [node.js](http://nodejs.com) and a couple nifty tools in node.

Out of all the cool tools in node my current favorite is the fork functionality to run multi-core, it allows me to spin up a bunch more threads based on the server I am running on (Linode), so I get 8 cores.

I recently updated this site and got some huge performance gains. It went from being able to handle ~1 million users a day to ~14 million users a day based on my stress testing.

# So how does this article get loaded?

First the system connects to github and requests my base data if it doesn't have it yet, that way it can load all the repositories I need to make this site work, currently only 1.

( I'm writing this post on my tablet and will commit->push to update my files )

Once the client has connected the server asks github for a list of files in a specific repository (FortuneFerret) and loads their metadata, once you click on an article it then pulls its contents from github (if it doesn't have a recently cached version available)

The file name is actually the title of the article (this makes writing concise titles important) for example this article's name is:

HowLevidehaan.comIsBuilt.md it inserts a space after each capital letter, I know I could go with something more fancy than title<->filename, but it serves my purpose and it allows me to update my pages easily, get comments on articles in github, and get pull requests on articles.


------------

## More Info

Please feel free to read the code, you will learn so much more.
