#Working towards great version control for content creators

##Hi, thank you for choosing this track.
My name is **Floor Drees**. I was actually born here, in Leiden.  
Two years ago I exchanged Rotterdam for Vienna to work at a startup that does 'stuff' with reviews and is **not** called Yelp. I had worked as a community manager for agencies and startups for 5 years, and here I'd make a little step up, becoming head of community management. Partly because I had been doing more or less the same thing over and over for years, ie community management, because I wanted to 'make stuff' again (I have a background in design) and because I worked closely together with the developers there, I decided I wanted to pick up on something new. That something new was learning to program. As this startup's stack used Ruby on Rails, there was no real decision process here on what language I'd be learning. Cool thing is that many of my developer coworkers had coached at Rails Girls events, and I was familiar with their program. I started going though their courses, in August last year, supported by one of my coworkers. Little later my company supported me to work as a junior developer one day a week, mainly documenting bugs talking to marketing and communication, and actually fixing bugs.   
I organized Rails Girls Rotterdam in January, [Rails Girls The Hague](http://railsgirls.com/thehague) 3 weeks ago, I co-organize the [Ruby user group meetups in Vienna](http://vienna-rb.at), the [PyLadies workshops in Vienna](http://www.meetup.com/PyLadies-Vienna/) and I co-organize the WordPress user group meetups in Vienna, although most of the credits for that one should go to Paolo Belcastro.   

I build and maintain(ed) multiple WordPress sites ever since I discovered blogging early 2008. Fun fact: back then I wrote for the group blog (on recruitment) from my dad. And as an art academy student I never really explored all this online content stuff so I'd actually email my blogs to him, and he'd post them on WordPress under my name.   

I currently work at [Usersnap](http://usersnap.com), a screenshot tool for web developers, that helps collect better bug reports. I promised them a shameless plug for [our WordPress plugin](http://wordpress.org/plugins/usersnap/), so here we go... Annnd it's over.  


##My problem with WordPress
As someone who incidentally writes about stuff with other people, I often encounter the same problem. You either email tiny changes to your article to the one who’s ultimately responsible for the website, which is bound to go wrong. Or you log into your CMS, make some changes to your piece and save it, while one of the other editors does the exact same thing, just using another shiny laptop. Changes get lost. Stuff gets added twice and you end up frustrated because the preview doesn’t reflect your work. Now this is annoying as it is, but if you program a bit on the side (like I do) and you use version control, you know that there is a solution for that. I'd love walk you through what I think would make a great version control tool for WordPress and test existing plugins by these requirements.

I use private repo's on GitHub to store my wp-files (not individual posts) and thus use version control for the sites I built with WordPress. And I always have a backup in 'the cloud'. I wish I could do the same for my posts.   

I'm not the only one:  
Loren Burton on how he's building [GitHub for Writers](http://madebyloren.com/github-for-writers).
  
"... despite how crucial GitHub is to the developer toolbox, I'm constantly wondering why the platform is limited to just code."  

Instead of building a GitHub 'for everyone/everything else' however, I want to see what's already out there that connects with WordPress, that I/we can help improve on. I'm lazy.  

"... there can be multiple pull requests and multiple versions of the code floating around simultaneously (thanks, Git!), but everything eventually ends up in single place (master branch)."  

[The limitations of GitHub for writers](http://www.chronicle.com/blogs/profhacker/the-limitations-of-github-for-writers/48299)  
[GitHub for teachers](http://www.coding2learn.org/blog/2013/07/12/github-for-teachers/)  
[I want a GitHub of science](http://www.marciovm.com/i-want-a-github-of-science/)

And then there was THE Wired article: [From Collaborative Coding to Wedding Invitations: GitHub Is Going Mainstream](http://www.wired.com/wiredenterprise/2013/09/github-for-anything/). The guy they refer to in their title is software engineer Bubby Rayber, who turned to GitHub to track and plan his wedding. “The open, collaborative workflow we have created for software development is so appealing that it’s gaining traction for non-software projects that require significant collaboration,” says GitHub cofounder and CEO Tom Preston-Werner.  

Last year, Twitter’s top lawyer, Benjamin Lee, used GitHub to draft a new licensing agreement for his company’s engineers, and before long, other GitHub users had fixed a handful of minor grammatical errors. Then Trishan Arul, head of business operations at Twitter cofounder Evan Williams’ startup incubator, Obvious, suggested some text that he wanted Lee to incorporate, and Lee did.

In a completely different realm, Adam Wood, music director of an Episcopal church in Texas, is uploading a compendium of Gregorian chants to GitHub. He thinks the service is the perfect place for choir directors to share and improve all kinds of music.

With 3.4 million users, the five-year-old site is a runaway hit in the hacker community, the go-to place for coders to show off pet projects and crowdsource any improvements. But the company has grander ambitions: It wants to change the way people work. It’s starting with software developers for sure, but maybe one day anyone who edits text in one form or another — lawyers, writers, and civil servants — will do it the GitHub way.   

To people who do not program, a visit to GitHub is a daunting run through the hacker jargon gauntlet. There are repositories, or “repos,” big chunks of code or text that get edited and “forked.” There are smaller snippets, called Gists. It’s tough for non-technical users to figure things out, but for engineers, this stuff is candy. Tech jargon: non-developers don't understand branches, forks, commits, rebasing, cloning, etc.. and they don't care to learn.
GitHub is moving Git functionality into the browser. GitHub diffs (changes in a file) are designed for code: line-by-line diffs instead of words, sentences, and paragraphs. But a little bird told me that this is changing.    

###WordPress 3.6 "Oscar"

Flagship feature (if you'd ask me) of [WordPress 3.6 "Oscar"](http://wordpress.org/news/2013/08/oscar/) is the revamped **Revisions**, **Post Locking** and **Augmented Autosave**:  
Revisions save every change and the new interface allows you to scroll easily through changes to see line-by-line who changed what and when. Post Locking and Augmented Autosave will especially be a boon to sites where more than a single author is working on a post. Each author now has their own autosave stream, which stores things locally as well as on the server (so much harder to lose something) and there’s an interface for taking over editing of a post.  

From the first word you write, WordPress saves every change. Text is highlighted as you scroll through revisions at lightning speed, so you can see what changes have been made along the way.  
It’s easy to compare two revisions from any point in time, and to restore a revision and go back to writing. No mistake is permanent.  
Autosaving is got heaps better; whether your power goes out, your browser crashes, or you lose your internet connection, your content is safe.  
Always know who’s editing with live updates that appear in the list of posts. And if someone leaves for lunch with a post open, you can take over where they left off.  

###Version Control the way I like it

I've used both Git and Subversion for my development projects, and decided for GitHub for it's open source culture and easy to manage process. A lot of the feature request will therefor have a GitHub flavor. You'll need to excuse me for being a fangirl. 

#####Forking / cloning  

Templating for posts. In the software environment, the term "fork" means you make an identical copy of something, that ends up as /me/forkedproject. Multiple users could fork a code base, or in our case a post or a page and make it their own. As in: use it to their use case, or improve on their version of your project and...  

#####Branches  & pull requests

... maybe send a pull request. As said, when editing a post, in the background, you'd actually be working on your local copy. You can suggest your changes to the admin of a group blog or website.  

#####Commenting on changes  

Commenting on changes, both your own' and others, helps to get everyone in the project on the same page - quite literally. You might want to explain why you deleted a whole paragraph, or why you find that cat picture less fitting. Rather than  using email for such things, why not keep it in one place? Your plugin installation / WordPress dashboard.  

#####Committing (naming changes)  

Potentially even committing your changes, 'single signing off', registering your alterations and takig responsibility for your changes.

##### Task lists (issues) with assigning possibilities

Task lists (issues) with assigning possibilities. Why use a bug trackers, a project management tool... and WordPress, right? Ok, for smaller blogs this might not even a pressing issue, but imagine if it would be possible!  

#####All in the termina-NATIVE app  

Phew! I was about to say terminal there... I need to keep in mind that I want to work towards something that's intuitive for content creators, especially the ones who are not necessarily tech savvy. 

#####Notifications?

I'd like to receive notifications when my blog mates sign of a change or respond to text that I've written or altered. Same goes for issues/tasks that get added and pull requests that get... pulled? But maybe I'm feature freaking here.   

I actually wanted to put 'broader range of markdown/syntax support' in here as well... but that's a whole different topic, maybe for a next WordCamp ;)   

####So... What's out there that slighty resembles what I want/need?

#####WP Document Revisions

**Requires:** 3.2 or higher  
**Compatible up to:** 3.6.1  
**Last Updated:** 2013-7-3
**Downloads:** 47,064  

4.9 out of 5 stars for 39 users  

[WP Document Revisions](http://wordpress.org/plugins/wp-document-revisions/) is a document management and version control plugin. Built for time-sensitive and mission-critical projects, teams can collaboratively edit files of any format -- text documents, spreadsheets, images, sheet music... anything -- all the while, seamlessly tracking the document's progress as it moves through your organization's existing workflow.

**WP Document Revisions is**  
A document management system (DMS), to track, store, and organize files of any format  
A collaboration tool to empower teams to collaboratively draft, edit, and refine documents  
A file hosting solution to publish and securely deliver files to a team, to clients, or to the public  

**The Vitals** 
Support for any file type (docs, spreadsheets, images, PDFs -- anything!)  
Provides a full file history in the form of a revision log, accessible via RSS  
Helps you track and organize documents as they move through your organization's existing workflow  
Each file gets a permanent, authenticated URL that always points to the latest version  
Each revision gets its own unique url (e.g.,TPS-Report-revision-3.doc) accessible only to those you deem  
Files are intuitively checked out and locked to prevent revisions from colliding  
Documents and Revisions shortcodes, Recently Revised Documents widget  
Integration with **Edit Flow**  
Recently Revised Documents Widget, shortcodes, and templating functions for front-end integration  

**Features Available via the Code Cookbook:**  

Audit Trail - creates check in / check out audit trail for all documents  
Taxonomy-based Permissions - allows setting user-level permissions based on a custom taxonomy such as department  
Third Party Encryption - example of how to integrate at rest encryption using third-party tools  
Rename Documents - changes all references to "Documents" in the interface to any label of your choosing  
State Change Notification - how to use document api to allow users to receive notification whenever documents change workflow state  
Bulk Import - how to batch import a directory (or other list) of files as documents  
Filetype Taxonomy - Adds support to filter by filetype  
Track Changes - Auto-generates and appends revision summaries for changes to taxonomies, title, and visibility  
Remove Workflow States - Completely removes Workflow state taxonomy backend and UI  
Change Tracker - Auto-generates and appends revision summaries for changes to taxonomies, title, and visibility  

#####Post Forking

**Requires:** 3.5 or higher  
**Compatible up to:** 3.6.1  
**Last Updated** 2013-9-26 
**Downloads:** 1,288  

5 out of 5 stars (for 13 users).  

[Post Forking](http://wordpress.org/plugins/post-forking/) allows users to "fork" or create an alternate version of content to foster a more collaborative approach to WordPress content curation. This can be used, for example, to allow external users (such as visitors to your site) or internal users (such as other authors) with the ability to submit proposed revisions. It can even be used on smaller or single-author sites to enable post authors to edit published posts without their changes appearing immediately.   
"If you're familiar with Git, or other decentralized version control systems, you're already familiar with WordPress post forking."  

**How might you use it?**  
Allowing users without edit or publish post capabilities to edit and submit changes to content (similar to GitHub’s pull request system)  
Collaborative editing (by resolving two users’ conflicted saves – Wired’s example)  
Saving draft changes of already-published content  
Scheduling pending changes to already-published content  

**How does it work?**  
When a user without the edit_post capability attempts to edit a given post, WordPress will automatically create a "fork" or alternate version of the post which they can freely edit. The edit screen will look just like the standard post editing interface that they are used to. When they're done, they simply click "submit for review." At this point, the fork goes into the standard WordPress moderation queue (just like any time an author without the publish_post capability submits a post), where an editor can review, and potentially approve the changes for publishing. If the changes can be automatically merged, the original post will be updated, otherwise, the editor will be presented with the ability to resolve the conflicting changes. All this is done using WordPress's built-in custom post type, revision, and diff functionality, so it should look familiar to most WordPress users.
Concepts  

**WordPress Post Forking introduces many of Git's well-established conventions to the WordPress world, and as a result, uses a unique vocabulary to describe what it does:**  
Post - Any WordPress post that uses the post_content field, including posts, pages, and custom post types  
Fork - Clone of a post intended for editing without disturbing the parent post  
Branch - Parallel versions of the same parent post, owned by the post author  
Merge - To push a fork's changes back into its parent post  
Conflict - When a post is forked if a given line is changed on the fork, and that same line is subsequently edited on the parent post prior to the merge, the post cannot be automatically merged, and the conflict is presented to the merger to resolve  

**Why this plugin?**  

[GitHub for Journalism — What WordPress Post Forking could do to Editorial Workflows](http://ben.balter.com/2012/02/28/github-for-journalism-what-wordpress-post-forking-could-do-to-editorial-workflows/)  

Nowadays, GitHub hosts more than just source code. Books, transcripts of talks and even whole constituents.   


"At Wired offices, you hear the question over and over again as we work on stories like the one you’re reading now: “Are you out of the story? I want to go in.” We have a version control problem. We publish Wired.com on WordPress. It’s a decent publishing tool, but when two people change a story at the same time, one of them doesn’t get her changes onto the final story. We published our GitHub story on GitHub because it was meta-cool. But we also did it to see if GitHub might actually help us solve our problem."
http://www.wired.com/wiredenterprise/2012/02/github-revisited/

"People were fixing the same problem over and over again. Some of their changes couldn’t be merged automatically, but they included good additions that should be considered. GitHub lets users describe the changes they’re making, but not everyone is precise when doing this. So you need to check closely to see what is really being changed."

The suggested change, in [GitHub for Journalism — What WordPress Post Forking could do to Editorial Workflows](http://ben.balter.com/2012/02/28/github-for-journalism-what-wordpress-post-forking-could-do-to-editorial-workflows/):  

User without the ability to edit an existing post has changes to make  
User “forks” the post, making any change they deem necessary  
When done, user attempts to merge changes back into the original  
Post goes into standard WordPress “pending review” workflow  
Editor is presented with diff (using the built-in diff engine), and can automatically accept changes (if there are no conflicts), or manually merge the two if necessary  
Post is re-published with updated content, revision logs merged to reflect history  


Extends WordPress’s existing revision system  
Clone existing posts, edit, and “republish”  
Schedule changes to posts, including taxonomies and metadata  
Pending changes diff view, front-end preview of changes  
Using WordPress’s pending-review system, integrates with existing plugins for notifications, management, etc.  
Ability to store “commit messages” with each post revision to explain to others what changes were made and why  
Automatically merges (non-conflicted) changes (based on existing diff engine)  
    - One sided changes – one overwrites the other  
    - Two sided non-conflict changes – automatically merge  
    - Conflicted changes – note conflicts in fork and prepare for re-merge  


#####Edit Flow
**Requires:** 3.4 or higher  
**Compatible up to:** 3.5.2  
**Last Updated:** 2013-1-31  
**Downloads:** 61,388  

4.9 out of 5 stars for 72 users  

[Edit Flow](http://wordpress.org/plugins/edit-flow/) empowers you to collaborate with your editorial team inside WordPress. We've made it modular so you can customize it to your needs:  

Calendar - A convenient month-by-month look at your content.  
Custom Statuses - Define the key stages to your workflow.  
Editorial Comments - Threaded commenting in the admin for private discussion between writers and editors.  
Editorial Metadata - Keep track of the important details.  
Notifications - Receive timely updates on the content you're following.  
Story Budget - View your upcoming content budget.  
User Groups - Keep your users organized by department or function.  


#####Revisionary

**Requires:** 3.0 or higher  
**Compatible up to:** 3.6.1  
**Last Updated:** 2013-8-19  
**Downloads:** 18,741  

4.7 out of 5 stars for 18 users.  

[Revisionary](http://wordpress.org/plugins/revisionary/). Have you ever wanted to allow certain users to submit changes to published content, with an editor reviewing those changes before publication? Doesn't it seem like setting a published post/page to a future date should schedule your changes to be published on that date, instead of unpublishing it until that date? Revisionary enables qualified users to submit changes to currently published posts or pages. Contributors also gain the ability to submit revisions to their own published content. These changes, if approved by an Editor, can be published immediately or scheduled for future publication.   

Pending Revisions allow designated users to suggest changes to a currently published post/page  
Scheduled Revisions allow you to specify future changes to published content (either via Pending Revision approval or directly by fully qualified author/editor)  
Enchanced Revision Management Form  
Front-end preview display of Pending / Scheduled Revisions with "Publish Now" link  
New WordPress role, "Revisor" is a moderated Editor  
Works with blog-wide WordPress Roles, or in conjunction with Press Permit or Role Scoper  


#####Duplicate Post

**Requires:** 3.0 or higher  
**Compatible up to:** 3.3.2  
**Last Updated:** 2012-5-4  
**Downloads:** 386,875  

4.8 out of 5 stars for 154 users  

[Duplicate Post](http://wordpress.org/plugins/duplicate-post/) clones posts and pages. This plugin allows to clone a post or page, or edit it as a new draft.  

In 'Edit Posts'/'Edit Pages', you can click on 'Clone' link below the post/page title: this will immediately create a copy and return to the list.  
In 'Edit Posts'/'Edit Pages', you can click on 'New Draft' link below the post/page title.  
On the post edit screen, you can click on 'Copy to a new draft' above "Cancel"/"Move to trash".  
While viewing a post as a logged in user, you can click on 'Copy to a new draft' as a dropdown link under "Edit Post" in the admin bar.  

2, 3 and 4 will lead to the edit page for the new draft: change what you want, click on 'Publish' and you're done.  

Pay attention to the new behaviour! The first way now allows you to clone a post with a single click, speeding up your work if you have many posts to duplicate.  

There is also a template tag, so you can put it in your templates and clone your posts/pages from the front-end. Clicking on the link will lead you to the edit page for the new draft, just like the admin bar link.  

In the Options page under Settings it is now possible to choose what to copy:  
the original post/page date  
the original post/page status (draft, published, pending), when cloning from the posts list  
the original post/page excerpt  
the original post/page attachments (actual files won't be copied)  
all the children of the original page  
which taxonomies and custom fields  

You can also set a prefix (or a suffix) to place before (or after) the title of the cloned post/page, and the roles allowed to clone posts or pages.  

####Monday is hackathon day, right?  

I'd love to help WordPress create version control for its users, or bring it to GitHub standards. But I need help for that. Please find me in the break if you'd like to work on this as well! I'm thinking about contributing to Post Forking (as it also integrates with Edit Flow), but if one of you is working on the next big thing, I'd love to help.  

###Thank you. 






