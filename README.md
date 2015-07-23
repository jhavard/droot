DROOT
=====

I'm always on the lookout for "better" ways of publishing sites.  I have tried everything from
big and nasty Java-based ECM systems with a convoluted web publishing workflow, to homebrew Lisp-based
blogs.  Recently, I decided to use static site generators, but there was one other option that almost
won out... use JSP and custom tags.  While JSP?  It works everywhere in a simple, self-contained bundle.
Actually, one of the open source CFML engines would have been easier, but they need a bit more ram than a
bare bones Tomcat instance.

So, DROOT, which is short for *Dumb ROOT*, is about as stupid simple as you can get.  Import
the tagdir, define the title, stuff some text in the special body tag, and then end it with a
tag that essentially renders the page.  This thing is practically codeless.

I'm not all that happy with needing to use *${pageContext.request.contextPath}* everywhere to get
the paths correct, but I guess that is a small price to pay.

The stock template for this project  was something I whipped up rather quickly while fooling around in
Adobe's DreamWeaver, to see if it has improved in any way over the years.  It certainly looks better,
but in some respects, it is less functional.  It no longer has any concept of trying to play nice with
anything other than straight HTML.  Then again, its template system solves the bulk of all problems one
typically wants to solve with a WCM system.  They also either hid or did away with the tag attribute
editing dialogs.  I figured that if I'm going to be forced to type code, I may as well use a text
editor I actually like.  So, no need for Dw, and then I made this.

