---
title: Setting Up Shiny Server Professional.
---
[Shiny Server](https://rstudio.com) is an awesome framework for reactive web application. I would even say, that it's the best and most mature out there right now in terms of reactivity. The Rstudio guys around Joe Cheng, Winston Chang, Hadley Wickham and all the others are pretty passionate when it comes to their promising framework and they have their reasons to do so.  

After playing around with the open source version for two years I finally was able to deploy a "real" application for one of my customers. It's a rather small app, with some knitr connectivity and other basic stuff, but it was (and still is) a really good experience. The application runs on a ec2 t2 micro instance (+ a sql server in the background) and eats almost none ressources. It's been up since August 2015 and there was no trouble so far.  

Unfortunately are (of course) some features missing in the open source version, so that you won't get around using the professional version of shiny server for larger projects - well I guess we can be happy that there is a possibility to use all the advanced functionaly, so I'm not complaining! However, at the moment I'm in communication with another customer who wants to implement shiny as the main (and only) internal (and to some extents external) reporting tool and the whole thing starts to develop as a pretty huge challenge for me.   
First: I have no idea, how much ressource will be actually needed for a server who should handle 100-150 people at any given time, second: how much traffic does the server need with 20-30 applications on it. The third aspect is of course: how much time and ressource will be needed to maintain all the apps? Is it possible to handle by one person? Two? Three? 
At the moment I'm pretty excited and really hope, that we will get the opportunity to start this project - I see quite a lot potential in it. 




