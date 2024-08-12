AUTHOR: Bryan
TITLE: MT4 cripples me and leaves me helpless
BASENAME: mt4_cripples_me_and_leaves_me
STATUS: Publish
ALLOW COMMENTS: 1
CONVERT BREAKS: __default__
ALLOW PINGS: 1
DATE: 09/06/2007 04:28:55 PM
-----
BODY:
Yesterday <a href="http://www.emilychang.com/go/ehub/app/ehub-analyzes-movable-type-4/">a piece I wrote about the new Movable Type 4</a> was posted on eHub. It was a story I asked for, but ultimately, I was unable to be as effective on the story as I'd like--mainly for very technical, mac-related reasons.

One of the things that really won me over when I was wrestling with switching in Korea was the relative ease with which you could create a development environment and test your sites and web applications locally on a Mac machine. I say relative because it did require some delving into concepts that I had been avoiding like the plague.

Now that I've got the new <a href="http://www.flickr.com/photos/leftsider/763948996/">MacBook</a>, I really was hoping to avoid the hassle of setting up the development environment all over again. I was actually considering working with Ruby on Rails just so that I could develop in <a href="http://locomotive.raaum.org/">Locomotive</a>, but instead I found the answer to my dreams, <a href="http://www.mamp.info/en/mamp.html">MAMP</a>.

Usually your typical web dev setup consists of Linux, Apache, mysql, and PHP (or Perl). A short acronym is LAMP; MAMP simply refers to using the Macintosh platform (which runs on linux). A neat little app that allowed me to develop and test in such an easy way was all my dreams come true.

In the next day or so I installed about eight different content management systems, blogging platforms, wikis and other goodies. It worked without a hitch. With the added fun of <a href="http://www.leftsider.com/leftsider/2007/05/coda.htm">working with Coda</a>, life was a bowl of pitted cherries.

Enter MT4. This blog runs on MT3, so I was eager to give the new version a test drive. It's seemed natural that I just write about it as I go. I downloaded the beta and went to install. Installation is a lot easier in this iteration, though not as nice as some of the other systems I'd just installed. Dropping the static files into MAMP's htdocs folder and the cgi files into the cgi-bin, I opened a browser and worked through the install.

Progress halted at a request for the DBI module. Hmm. Oh wait; My <a href="http://zerokarmaleft.43people.com/">good buddy</a> showed me a little magic called CPAN... That should do the trick!

Well it would if I could actually MAKE the stupid module once installed. I can't, for the life of me, seem to get this module installed. It would seem a couple other people have had similar issues:

<a href="http://forum.mamp.info/viewtopic.php?t=1204&highlight=dbi">http://forum.mamp.info/viewtopic.php?t=1204&highlight=dbi</a>
<a href="http://forum.mamp.info/viewtopic.php?t=1131&highlight=dbi">http://forum.mamp.info/viewtopic.php?t=1131&highlight=dbi</a>

And that this may be an OS X issue:

<a href="http://www.cpanforum.com/posts/859">http://www.cpanforum.com/posts/859</a>
<a href="http://www.thescripts.com/forum/thread676055.html">http://www.thescripts.com/forum/thread676055.html</a>

But I can't seem to find a definite, consistent answer to correcting.

I'm tempted to just go the old way and install mysql, but thinking about that made me wonder where the location of MAMP's mysql is--would I lose the databases from my other web apps if I did that--and if Movable Type is looking in the correct location for the DBI module.

Unfortunately I'm not finding very many answers. And, of course, knowledgeable voices in this regard are in short supply. So, my return to blogging with regularity has been attacked again. I ended up installing MT4 and testing it from my webhost just to get the eHub piece out of the way. 

Since I want to upgrade this site and do some design diddling as well, this problem has been taking up huge portions of my day. I'll try to give posts some equal time. I'll also update this post for future generations if I ever do find an explainable solution.
-----
EXTENDED BODY:

-----
EXCERPT:

-----
KEYWORDS:

-----

COMMENT:
AUTHOR: Edward Cho
EMAIL: zerokarmaleft@gmail.com
IP: 24.253.220.246
URL: http://rabiddustbunnies.blogspot.com
DATE: 09/07/2007 07:32:49 AM
Hmm, wish I could help with the Perl DBI install issue, but I really don't know where to start since I don't have hands-on access to a Mac anymore.  My guess (i.e. I'm totally talking out of my ass here) is that a typical CPAN module's install script is going to try and copy files to OSX's file hierarchy.  While MAMP, b/c it includes some duplicate software that exists already with OSX shipped, probably installs itself as a substrate.  A quick glace at MAMP's website didn't immediately confirm this, but Fink and DarwinPorts use this approach to avoid file collisions.  If so, the trick is to install the Perl DBI module into MAMP's file hierarchy.
-----

COMMENT:
AUTHOR: Leftsider
EMAIL: leftsider@gmail.com
IP: 68.50.104.75
URL: 
DATE: 09/07/2007 10:05:37 AM
At least you're thinking in the same direction. I gave a cursory glance over what's inside the MAMP folder. I'll give it a more thorough comb-over maybe this weekend.
-----


