[![Build Status](https://travis-ci.org/DockDogs/dockdogs-office-sops.svg?branch=master)](https://travis-ci.org/DockDogs/dockdogs-office-sops)

[![Documentation Status](http://readthedocs.org/projects/dd-sops/badge/)](http://dd-sops.readthedocs.org/en/latest/)

Pre-requesites
==============

-   [Git]
-   [Sphinx]
-   Python 2.x
-   Pip (for using/installing Sphinx)
-   Text editor such as Atom, Notepad++, or SublimeText.
-   Terminal/Powershell access (iTerm2, Terminal.app, etc.)
-   Git Desktop client *(if you prefer a GUI instead of a shell prompt). Suggested applications would be Github Desktop Client, Sourcetree, or Tower (Mac OS X Only)*.

Checkout Documentation for Editing
==================================

How to Edit
===========

-   Edit files in `source` folder using a text editor such as Atom, SublimeText, or Notepad++.
-   Files are written in `reStructuredText` or `Markdown` syntax. Learn more about `Markdown` syntax at at [DaringFireball] or [Markdown Cheatsheet]. Github also has an official [Markdown reference guide].

Build & Deployment Status
=========================

[![Build Status](https://travis-ci.org/DockDogs/dockdogs-office-sops.svg?branch=master)](https://travis-ci.org/DockDogs/dockdogs-office-sops)

[![Documentation Status](http://readthedocs.org/projects/dd-sops/badge/?version=latest)](http://dd-sops.readthedocs.org/en/latest/?badge=latest)

Build Testing & Deployment
==========================
* All commits pushed to the Docs are first sent for CI Testing via [Travis-CI](https://travis-ci.org/DockDogs/dockdogs-office-sops)
* If [Travis-CI](https://travis-ci.org/DockDogs/dockdogs-office-sops) build passes a ```Git Hook``` runs to inform ```Read The Docs``` to initiate a new build.
* If the new build succeeds on Read The Docs then it is live. 

Getting a Specific Release & Viewing All Releases
=================================================

-   [View Releases]
-   [Download Latest PDF Build]

License & Copyright
===================

-   Copyright 2016, All Rights Reserved - [DockDogs Worldwide].

Contributors
============

-   [Brian J King]

  [Git]: http://github.com
  [Sphinx]: http://www.sphinx-doc.org/en/stable/
  [DaringFireball]: https://daringfireball.net/projects/markdown/
  [Markdown Cheatsheet]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
  [Markdown reference guide]: https://help.github.com/articles/markdown-basics/
  [View Releases]: https://github.com/DockDogs/dockdogs-office-sops/releases
  [Download Latest PDF Build]: http://readthedocs.org/projects/dd-sops/downloads/pdf/latest/
  [DockDogs Worldwide]: http://dockdogs.com
  [Brian J King]: http://github.com/brianjking
