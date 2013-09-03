###Working towards great version control for content creators

As someone who incidentally writes about stuff with other people, I often encounter the same problem. You either email tiny changes to your article to the one who’s ultimately responsible for the website, which is bound to go wrong. Or you log into your CMS, make some changes to your piece and save it, while one of the other editors does the exact same thing, just using another shiny laptop. Changes get lost. Stuff gets added twice and you end up frustrated because the preview doesn’t reflect your work. Now this is annoying as it is, but if you program a bit on the side (like I do) and you use version control, you know that there is a solution for that. For WordCamp I'd love to gather my thoughts on what would make a great version control tool for WordPress and test [existing plugins][1] by these requirements.

I use private repo's on GitHub to store my wp-files (not individual posts) and thus use version control for the sites I built with WordPress. And I always have a backup in 'the cloud'. I wish I could do the same for my posts.   

I'm not the only one:  
Loren Burton on how he's building [GitHub for Writers][10].
  
"... despite how crucial GitHub is to the developer toolbox, I'm constantly wondering why the platform is limited to just code."  

Instead of building a GitHub 'for everyone else' however, I want to see what's already out there that connects with WordPress, that I/we can help improve on.  

"... there can be multiple pull requests and multiple versions of the code floating around simultaneously (thanks, Git!), but everything eventually ends up in single place (master branch)."  

[The limitations of GitHub for writers][11]  
[GitHub for teachers][12]  
[I want a GitHub of science][13]  


From Collaborative Coding to Wedding Invitations: GitHub Is Going Mainstream  
http://www.wired.com/wiredenterprise/2013/09/github-for-anything/  

Software engineer Bubby Rayber, who turned to GitHub to track and plan his wedding.  

“The open, collaborative workflow we have created for software development is so appealing that it’s gaining traction for non-software projects that require significant collaboration,” says GitHub cofounder and CEO Tom Preston-Werner.  

Last year, Twitter’s top lawyer, Benjamin Lee, used GitHub to draft a new licensing agreement for his company’s engineers, and before long, other GitHub users had fixed a handful of minor grammatical errors. Then Trishan Arul, head of business operations at Twitter cofounder Evan Williams’ startup incubator, Obvious, suggested some text that he wanted Lee to incorporate, and Lee did.

In a completely different realm, Adam Wood, music director of an Episcopal church in Texas, is uploading a compendium of Gregorian chants to GitHub. He thinks the service is the perfect place for choir directors to share and improve all kinds of music.

With 3.4 million users, the five-year-old site is a runaway hit in the hacker community, the go-to place for coders to show off pet projects and crowdsource any improvements. But the company has grander ambitions: It wants to change the way people work. It’s starting with software developers for sure, but maybe one day anyone who edits text in one form or another — lawyers, writers, and civil servants — will do it the GitHub way.   

To people who do not program, a visit to GitHub is a daunting run through the hacker jargon gauntlet. There are repositories, or “repos,” big chunks of code or text that get edited and “forked.” There are smaller snippets, called Gists. It’s tough for non-technical users to figure things out, but for engineers, this stuff is candy.   



BUT  

####WordPress 3.6 "Oscar"

Flagship feature (if you'd ask me) of [WordPress 3.6 "Oscar"][2] is the revamped **Revisions**, **Post Locking** and **Augmented Autosave**:  
"Revisions save every change and the new interface allows you to scroll easily through changes to see line-by-line who changed what and when."  
"Post Locking and Augmented Autosave will especially be a boon to sites where more than a single author is working on a post. Each author now has their own autosave stream, which stores things locally as well as on the server (so much harder to lose something) and there’s an interface for taking over editing of a post, as demonstrated beautifully by our bearded buddies in the video above."  

####Version Control the way I like it

I've used both Git and Subversion for my development projects, and decided for GitHub for it's open source culture and easy to manage process. A lot of the feature request will therefor have a GitHub flavor. You'll need to excuse me for being a fangirl. 

#####Forking / cloning  

Templating for posts. 

#####Branches  & pull requests

When editing a post, in the background, you're working on your local copy. 

#####Commenting on changes  

Both your own' and others.

#####Committing (naming changes)  

'single sign off'

##### Task lists (issues) with assigning possibilities

Bug trackers, project management tool... and WordPress. 

#####All in the termina-NATIVE app  

Phew! I was about to say terminal there... Need to keep in mind that I want to work towards something that's intuitive for content creators, especially the ones who are not necessarily tech savvy. 

#####Notifications?

Tech jargon: non-developers don't understand branches, forks, commits, rebasing, cloning, etc.. and they don't care to learn.
GitHub is moving Git functionality into the browser. GitHub diffs (changes in a file) are designed for code: line-by-line diffs instead of words, sentences, and paragraphs. But a little bird told me that this is changing.  

teams, issues, pull requests, discovery, project management  
In-browser editor  
broader range of markdown/syntax support  

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

Nowadays, GitHub hosts more than just source code. Books, transcripts of talks and even whole constituents.   


"At Wired offices, you hear the question over and over again as we work on stories like the one you’re reading now: “Are you out of the story? I want to go in.” We have a version control problem. We publish Wired.com on WordPress. It’s a decent publishing tool, but when two people change a story at the same time, one of them doesn’t get her changes onto the final story. We published our GitHub story on GitHub because it was meta-cool. But we also did it to see if GitHub might actually help us solve our problem."
http://www.wired.com/wiredenterprise/2012/02/github-revisited/

"People were fixing the same problem over and over again. Some of their changes couldn’t be merged automatically, but they included good additions that should be considered. GitHub lets users describe the changes they’re making, but not everyone is precise when doing this. So you need to check closely to see what is really being changed."

The suggested change, in [GitHub for Journalism — What WordPress Post Forking could do to Editorial Workflows][5]:  

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



**Project Status**  
This version constitutes an initial release designed to showcase the plugin's core functionality and is intended to be improved upon with additional features and refinements as the project evolves. Please consider contributing your time to help improve the project.  

**More Information**  
For more information, or to contribute to this documentation, please visit the [Post Forking project wiki][6].  

#####Edit Flow
**Requires:** 3.4 or higher  
**Compatible up to:** 3.5.2  
**Last Updated:** 2013-1-31  
**Downloads:** 59,539  

4.9 out of 5 stars for 72 users  

[Edit Flow][7] empowers you to collaborate with your editorial team inside WordPress. We've made it modular so you can customize it to your needs:  

Calendar - A convenient month-by-month look at your content.  
Custom Statuses - Define the key stages to your workflow.  
Editorial Comments - Threaded commenting in the admin for private discussion between writers and editors.  
Editorial Metadata - Keep track of the important details.  
Notifications - Receive timely updates on the content you're following.  
Story Budget - View your upcoming content budget.  
User Groups - Keep your users organized by department or function.  

More details for each feature, screenshots and documentation can be found on our website.  

#####Revisionary

**Requires:** 3.0 or higher  
**Compatible up to:** 3.6  
**Last Updated:** 2013-8-19  
**Downloads:** 17,757  

4.7 out of 5 stars for 18 users.  

[Revisionary][8]. Have you ever wanted to allow certain users to submit changes to published content, with an editor reviewing those changes before publication?  

Doesn't it seem like setting a published post/page to a future date should schedule your changes to be published on that date, instead of unpublishing it until that date?  

Revisionary enables qualified users to submit changes to currently published posts or pages. Contributors also gain the ability to submit revisions to their own published content. These changes, if approved by an Editor, can be published immediately or scheduled for future publication.  
Partial Feature List

Pending Revisions allow designated users to suggest changes to a currently published post/page  
Scheduled Revisions allow you to specify future changes to published content (either via Pending Revision approval or directly by fully qualified author/editor)  
Enchanced Revision Management Form  
Front-end preview display of Pending / Scheduled Revisions with "Publish Now" link  
New WordPress role, "Revisor" is a moderated Editor  
Works with blog-wide WordPress Roles, or in conjunction with Press Permit or Role Scoper  


#####Duplicate Post

[Duplicate Post][9]

**Requires:** 3.0 or higher  
**Compatible up to:** 3.3.2  
**Last Updated:** 2012-5-4  
**Downloads:** 371,136  

4.8 out of 5 stars for 154 users  

Clone posts and pages.  

This plugin allows to clone a post or page, or edit it as a new draft.  

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

If you want to contribute to translate the plugin in languages other than English, there is a GlotPress translation project available (no registration required! — You can also send me an e-mail using the form on my website).  


####Monday is hackathon day, right?  

I'd love to help WordPress create version control for its users, or bring it to GitHub standards. But I need help for that. Please find me in the break if you'd like to work on this as well! 

[1]: http://wordpress.org/plugins/tags/version-control
[2]: http://wordpress.org/news/2013/08/oscar/
[3]: http://wordpress.org/plugins/wp-document-revisions/
[4]: http://wordpress.org/plugins/post-forking/
[5]: http://ben.balter.com/2012/02/28/github-for-journalism-what-wordpress-post-forking-could-do-to-editorial-workflows/
[6]: https://github.com/post-forking/post-forking/wiki
[7]: http://wordpress.org/plugins/edit-flow/  
[8]: http://wordpress.org/plugins/revisionary/
[9]: http://wordpress.org/plugins/duplicate-post/  
[10]: http://madebyloren.com/github-for-writers
[11]: http://www.chronicle.com/blogs/profhacker/the-limitations-of-github-for-writers/48299  
[12]: http://www.coding2learn.org/blog/2013/07/12/github-for-teachers/
[13]: http://www.marciovm.com/i-want-a-github-of-science/  
