** "Minimal" (ahem...) code for inducing a scroll-prohibiting bug in Firefox 58+**

The file orbit_controls.html is a near-standard example of using the OrbitControls.js from the three.js project.  The only thing I have added is 50 lines of html saying "Hello1", "Hello2" etc. to the top of the page. With that many lines on the page, a need for scrolling arises. But this scrolling is not possible in Firefox 58, while it was perfectly possible in Firefox 57. Thus there is a regression bug in Firefox.
Do note thar the actual orbit controls example visualisation can't be seen, as it is placed at the bottom of the page, below the 50 lines... 

The challenge is to reduce the code of this bug-inducing example. The Firefox bug manager has asked for that. I know very little about the internals of three.js and OrbitControls.js. Thus I'm asking for help from the three.js developers on how to reduce the code size for this bug-example, while keeping the bug-inducing behavior.

This is the Firrefox bug on Bugzilla: https://bugzilla.mozilla.org/show_bug.cgi?id=1418442
