---
title: 'PEP 830: Add timestamps to exceptions and tracebacks'
url: https://peps.python.org/pep-0830/
date: '2026-03-15'
author: Gregory P. Smith (greg@krypto.org)
feed_url: https://peps.python.org/peps.rss
---
This PEP adds an optional __timestamp_ns__ attribute to BaseException that records when the exception was instantiated with no observable overhead. When enabled via environment variable or command-line flag, formatted tracebacks display this timestamp alongside the exception message.
