---
title: Setting Up Hakyll
author: Darius
---
I've finally found some time to set up my personal small and lightweight website using Hakyll. Following the [official installation instructions](https://jaspervdj.be/hakyll/tutorials/01-installation.html) would definitely suffice, but since it's nice to have other peoples opinions and tutorials around, I'm giving you a short guide on how to set up everything by yourself.  

Installation
------------

Hakyll is written in Haskell and therefore it's necessary to have the compiler installed, the easiest way to do so is probably using the command line:  

> \$ sudo apt-get install haskell-platform  

This will install the so called [Haskell Platform](https://www.haskell.org/platform/), which is advertised to have "batteries included". Its basically consists of ghc, cabal and some additional packages.

We also need to install [Stack](http://docs.haskellstack.org/en/stable/README/), the best way is probably to follow the [official instructions](http://docs.haskellstack.org/en/stable/README/).

After everything is installed nicely we just need to shoot the following commands into our command line:

> \$ stack install hakyll  
> \$ hakyll-init \<mySite\>  && cd \<mySite\>  
> \$ stack build  
> \$ stack exec site build  
> \$ stack exec site watch  

These commands basically install hakyll, initialize it in a new project directory *mySite* and build the site for you. The last command starts the integrated webserver and launches a browser instance on <a href="localhost:8000">localhost:8000</a> to take a first look at your newly compiled website.  

Further configurations can be done within the *site.hs* file inside your *mySite* directory. 

Writing new blog posts
----------------------

Adding new posts is pretty simple and can be done by creating a markdown file within the *post/* subdirectory with this simple markdown layout:

> \-\-\-  
> title: My Blog Title  
> author: My Name  
> date: 2000-12-24  
> \-\-\-  
> text

the markdown file will be then compiled and rendered according to the settings you made. (or the basic setting, if you haven't changed anything yet)  

That should be about it! If you didn't understand any specific part, just contact me and I'll try to help out.
