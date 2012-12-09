git-share
=========
A simple tool to backup, share & restore git stashes

Why?
====
* Needed to format my work's laptop and had ~10 stashes didn't want to loose.
* Sometimes I could use a tool like this to share stashes between work-home.

Install
=======
* The tool requires git>=1.8
* Just place git-share in a place PATH accesible so you can run it as a git command.

Features
========
* Works with submodules
* Can handle conflicts

Usage
=====
1. git share stash backup [DIR]    backup all stashes to DIR or default ./git-share_stash (@origin_machine/git_project)
2. Share the directory full of stashes!
3. git share stash restore [DIR]   restore all stashes from DIR or default ./git-share_stash (@target_machine/git_project)

Things you may want to consider
===============================

* The tool will restore the stash over the current branch and not the original one, so you may have conflicts.
* The tool won't create paths recursively at the provided DIR, so make sure the parent of you DIR exists.
