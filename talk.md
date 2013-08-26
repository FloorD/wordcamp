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

####So... What's out there?

#####WP Document Revisions

**Requires:** 3.2 or higher  
**Compatible up to:** 3.6  
**Last Updated:** 2013-7-  3
**Downloads:** 44,661  

4.9 out of 5 stars for 38 users  

[WP Document Revisions][3] is a document management and version control plugin. Built for time-sensitive and mission-critical projects, teams can collaboratively edit files of any format -- text documents, spreadsheets, images, sheet music... anything -- all the while, seamlessly tracking the document's progress as it moves through your organization's existing workflow.

**WP Document Revisions is three things:**  

A document management system (DMS), to track, store, and organize files of any format  
A collaboration tool to empower teams to collaboratively draft, edit, and refine documents  
A file hosting solution to publish and securely deliver files to a team, to clients, or to the public  

Powerful Collaboration Tools - With great power does not have to come great complexity. Based on a simple philosophy of putting powerful but intuitive tools in the hands of managers and content creators, WP Document Revisions leverages many of the essential WordPress features that, for more than eight years, have been tested and proven across countless industries -- posts, attachments, revisions, taxonomies, authentication, and permalinks -- to make collaborating on the creation and publication of documents a natural endeavor. Think of it as an open-source and more intuitive version of the popular Microsoft collaboration suite, Sharepoint.  

Document History - At each step of the authoring process, WP Document Revisions gives you an instant snapshot of your team's progress and the document's history. It even gives you the option to revert back to a previous revision -- so don't fret if you make a mistake -- or receive updates on changes to the document right in your favorite feed reader.  

Access Control - Each document is given a persistent URL (e.g., yourcompany.com/documents/2011/08/TPS-Report.doc) which can be private (securely delivered only to members of your organization), password protected (available only to those you select such as clients or contractors), or public (published and hosted for the world to see). If you catch a typo and upload a new version, that URL will continue to point to the latest version, regardless of how many changes you make.  

Enterprise Security - Worried about storing propriety or sensitive information? WP Document Revisions was built from the first line of code with government- and enterprise-grade security in mind. Each file is masked behind an anonymous 128-bit MD5 hash as soon as it touches the server, and requests for files are transparently routed through WordPress's time-tested URL rewriting, authentication, and permission systems (which can even integrate with existing enterprise active directory or LDAP servers). Need more security? WP Document Revisions allows you to store documents in a folder above the htdocs or public_html web root, further ensuring that only those you authorize have access to your work.  

Customization - WP Document Revisions recognizes that no two teams are identical, and as a result, molds to your firm's needs, not the other way around. Need to track additional information associated with a document? Departments, editors, issues, sections, even arbitrary key-value pairs -- whatever you can throw at it, it can handle. Development and customization costs are further minimized by its extensive plugin API, and the WordPress Custom Taxonomy Generator makes it easy for even the uninitiated to add custom taxonomies to documents. Need an audit trail to track check-ins and check-outs? User-level permissions based on the document's state or another custom taxonomy? Support for third-party encryption? Check out the WP Document Revisions Code Cookbook for sample code. Looking for even more advanced control of your workflow? WP Document Revisions will detect the popular workflow plugin Edit Flow, if installed, and will automatically pull Edit Flow’s advanced workflow management tools into WP Document Revisions. Simply put, virtually every aspect of the plugin's functionality from workflow states to user-level permissions can be fully customized to your team's unique needs.  

Future Proof - Switching costs a concern? WP Document Revisions is built with tomorrow's uncertainty in mind. Equally at home in an in-house server room as it is in the cloud, moving individual files or entire document repositories in and out of WP Document Revisions is a breeze (history and all). And since the software is open-source, you can easily add tools to automate the process of moving to or integrating with future third-party systems.  

**The Vitals:** 

Support for any file type (docs, spreadsheets, images, PDFs -- anything!)  
Securely stores unlimited revisions of your business's essential files  
Provides a full file history in the form of a revision log, accessible via RSS  
Helps you track and organize documents as they move through your organization's existing workflow  
Each file gets a permanent, authenticated URL that always points to the latest version  
Each revision gets its own unique url (e.g.,TPS-Report-revision-3.doc) accessible only to those you deem  
Files are intuitively checked out and locked to prevent revisions from colliding  
Toggle documents between public, private, and password protected with a single mouse click  
Runs in-house or in the cloud  
Secure: filenames are hashed on upload and files are only accessible through WordPress's proven authentication system  
Can move document upload folder to location outside of web root to further ensure government- and enterprise-grade security  
Documents and Revisions shortcodes, Recently Revised Documents widget  
Multisite and Windows (XAMPP) support  
French and Spanish language support (easily translated to your language)  
Integration with Edit Flow  
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

**Translations:**  
French, Spanish, Norwegian, German, Chinese, Swedish, Czech, Italian, Russian, Dutch.

WP Document Revisions was developed by a law student and a business student with a grant from Google, and in close coordination with and under the watchful eye of WordPress.org's lead developers (Although neither relationship should imply an endorsement). Special thanks to Jon Cave, Aaron Jorbin, Mitcho Erlewine, and Andrew Nacin for their guidance.

#####Post Forking

**Requires:** 3.4 or higher  
**Compatible up to:** 3.5.2  
**Last Updated** 2012-9-30  
**Downloads:** 1,012  

5 out of 5 stars (for 13 users).  

[Post Forking][4] allows users to "fork" or create an alternate version of content to foster a more collaborative approach to WordPress.  

WordPress Post Forking allows users to "fork" or create an alternate version of content to foster a more collaborative approach to WordPress content curation. This can be used, for example, to allow external users (such as visitors to your site) or internal users (such as other authors) with the ability to submit proposed revisions. It can even be used on smaller or single-author sites to enable post authors to edit published posts without their changes appearing immediately. If you're familiar with Git, or other decentralized version control systems, you're already familiar with WordPress post forking.  

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

[GitHub for Journalism — What WordPress Post Forking could do to Editorial Workflows][5]  



**Project Status**  
This version constitutes an initial release designed to showcase the plugin's core functionality and is intended to be improved upon with additional features and refinements as the project evolves. Please consider contributing your time to help improve the project.  

**More Information**  
For more information, or to contribute to this documentation, please visit the [Post Forking project wiki][6].  

####Monday is hackathon day, right?  

I'd love to help WordPress create version control for its users, or bring it to GitHub standards. But I need help for that. Please find me in the break if you'd like to work on this as well! 

[1]: http://wordpress.org/plugins/tags/version-control
[2]: http://wordpress.org/news/2013/08/oscar/
[3]: http://wordpress.org/plugins/wp-document-revisions/
[4]: http://wordpress.org/plugins/post-forking/
[5]: http://ben.balter.com/2012/02/28/github-for-journalism-what-wordpress-post-forking-could-do-to-editorial-workflows/
[6]: https://github.com/post-forking/post-forking/wiki