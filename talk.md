###Working towards great version control for content creators

As someone who incidentally writes about stuff with other people, I often encounter the same problem. You either email tiny changes to your article to the one who’s ultimately responsible for the website, which is bound to go wrong. Or you log into your CMS, make some changes to your piece and save it, while one of the other editors does the exact same thing, just using another shiny laptop. Changes get lost. Stuff gets added twice and you end up frustrated because the preview doesn’t reflect your work. Now this is annoying as it is, but if you program a bit on the side (like I do) and you use version control, you know that there is a solution for that. For WordCamp I'd love to gather my thoughts on what would make a great version control tool for WordPress and test [existing plugins][1] by these requirements.

I use private repo's on GitHub to store my wp-files (not individual posts) and thus use version control for the sites I built with WordPress. And I always have a backup in 'the cloud'. I wish I could do the same for my posts.   

####WordPress 3.6 "Oscar"

Flagship feature (if you'd ask me) of [WordPress 3.6 "Oscar"][2] is the revamped **Revisions**, **Post Locking** and **Augmented Autosave**:  
"Revisions save every change and the new interface allows you to scroll easily through changes to see line-by-line who changed what and when."  
"Post Locking and Augmented Autosave will especially be a boon to sites where more than a single author is working on a post. Each author now has their own autosave stream, which stores things locally as well as on the server (so much harder to lose something) and there’s an interface for taking over editing of a post, as demonstrated beautifully by our bearded buddies in the video above."  

####Version Control the way I like it

I've used both Git and Subversion for my development projects, and decided for GitHub for it's open source culture and easy to manage process. A lot of the feature request will therefor have a GitHub flavor. You'll need to excuse me for being a fangirl. 

#####Forking / cloning  

Templating for posts. 

#####Branches  

When editing a post, in the background, you're working on your local copy. 

#####Commenting on changes  

Both your own' and others.

#####Committing (naming changes)  

'single sign off'

##### Task lists (issues) with assigning possibilities

Bug trackers, project management tool... and WordPress. 

#####All in the termina-NATIVE app  

Phew! I was about to say terminal there... Need to keep in mind that I want to work towards something that's intuitive for content creators, especially the ones who are not necessarily tech savvy. 

####Monday is hackathon day, right?  

I'd love to help WordPress create version control for its users, or bring it to GitHub standards. But I need help for that. Please find me in the break if you'd like to work on this as well! 

[1]: http://wordpress.org/plugins/tags/version-control
[2]: http://wordpress.org/news/2013/08/oscar/
[3]: http://wordpress.org/plugins/wp-document-revisions/
[4]: http://wordpress.org/plugins/post-forking/