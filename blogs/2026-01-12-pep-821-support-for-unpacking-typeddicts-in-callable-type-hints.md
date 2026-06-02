---
title: 'PEP 821: Support for unpacking TypedDicts in Callable type hints'
url: https://peps.python.org/pep-0821/
date: '2026-01-12'
author: Daniel Sperber (github.blurry@9ox.net)
feed_url: https://peps.python.org/peps.rss
---
This PEP proposes allowing Unpack[TypedDict] in the parameter list inside Callable, enabling concise and type-safe ways to describe keyword-only callable signatures. Currently, Callable assumes positional-only parameters, and typing keyword-only functions requires verbose callback protocols. With this proposal, the keyword structure defined by a TypedDict can be reused directly in Callable.
