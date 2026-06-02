---
title: 'PEP 829: Package Startup Configuration Files'
url: https://peps.python.org/pep-0829/
date: '2026-03-31'
author: Barry Warsaw (barry@python.org)
feed_url: https://peps.python.org/peps.rss
---
This PEP changes the way packages influence Python’s startup process. Previously controlled through legacy .pth files parsed and executed by the site.py file during interpreter startup, such files are used to extend sys.path and execute package initialization code before control is passed to the first line of user code.
