gunrack
=======

Stateful shepherding of many gunicorns.  Think of a bookshelf.  The frame is the Linux box.  The shelves are the DB, web proxy, memcached etc.  The application servers are the books.  This package is a bundle of tools, instructions, and parts.

problem
=======

Setting up a good clean webserver with the common Django apps is tedious.  A ton of experience is required to use all of the little tricks that make administration streamlined.  Just because a project is small doesn't mean it should be badly organized.  When documenting something, it makes as much sense to go ahead and automate it, preferably in a way that changing the automation can be retroactively applied to existing installations.

Goals
=====

+   Bring a blank Arch Linux box into a sane state with ssh keys and an admin user
+   Daemons are installed or not, support modular configs ( conf.d style ) where possible.  System package managers preferred for now.
+   Applications (Python for now) live in virtualenvs, use pip, and communicate with Daemons in uniform manner  
+   Django project is default install, using Python's templating to replace $variables like $project_name
+   Install sensible default apps and performant DB connectors e.g. South and django-psycopg2-pool
+   Tar up projects with keys to quickly spread the love to new team members
+   Basic monitoring and notifications to know when things are bad
+   Basic performance testing to 
+   Basic security tools like AIDE and grsec to provide fail-well security.

