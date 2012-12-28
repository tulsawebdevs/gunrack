Gunrack
=======

Stateful shepherding of many gunicorns.  Start python web apps faster, rightier, and more flexiblier.  Escape cargo-cult practices, learning curves, and bad memory.  Documentation through automation.  Do it fast.  Do it right.  Do it a lot.

Goals
=====

+   Bootstrap SSH, salt, and package manager on a new host
+   Modular (conf.d style) daemon setups so that running new applications on host is trivial
+   Applications (Python for now) live in virtualenvs, use pip, and communicate with Daemons in uniform manner  
+   Many "Guns" which are sensible templates for new projects.  "Racking" a gun results in a useable host and a tarball with everything needed to admin/develop
+   Basic monitoring and notifications to know when things are bad
+   Basic security tools like AIDE and grsec to provide fail-well security.  More on this later.

First Steps
===========

+   There is no salt.  There is no main directory structure.  All work so far is fabic and should be submitted to salt.
+   Need a blog for documenting design decisions.
+   Sphinx docs.
