---
title: 'PEP 825: Wheel Variants: Package Format'
url: https://peps.python.org/pep-0825/
date: '2026-02-17'
author: Jonathan Dekhtiar (jonathan@dekhtiar.com), Michał Górny (mgorny@quansight.com),
  Konstantin Schütze (konstin@mailbox.org), Ralf Gommers (ralf.gommers@gmail.com),
  Andrey Talman (atalman@meta.com), Charlie Marsh (charlie@astral.sh), Michael Sarahan
  (msarahan@gmail.com), Eli Uriegas (eliuriegas@meta.com), Barry Warsaw (barry@python.org),
  Donald Stufft (donald@stufft.io), Andy R. Terrel (andy.terrel@gmail.com)
feed_url: https://peps.python.org/peps.rss
---
This PEP proposes variant wheels, an extension to packaging:specifications/binary-distribution-format that permits building multiple variants of the same package while embedding additional compatibility data. The specific properties are stored inside the wheel, and expressed via a human-readable variant label in the filename, which is then mapped to the actual properties via a separately hosted JSON mapping. This aims to make {tool} install {package} capable of selecting the most appropriate variant of packages where additional compatibility dimensions such as GPU support need to be accounted for.
