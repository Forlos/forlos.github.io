+++
title = "Reverse engineering game archives - part 0 Introduction"
lastmod = 2020-10-20T20:55:14+02:00
tags = ["reverse engineering"]
draft = true
+++

This series of blog posts will try to explain process of reverse engineering game archives(or probably any archive you will come across).

If you ever wondered how to dump and make modifications to game files for modding or translation purposes then this should be a good place to start.

Articles will go from beginner level, starting with explaining thought process when trying to understand foreign file format and gradually come to harder things like anti reverse engineering and anti debugging techniques.

Articles should come with real world examples that I came across when reversing archives myself.

Also at the end of each post I will try to come with some exercises so you can apply your new skills and knowledge and test yourself.

Tools I will be using:

-   [Python 3](https://www.python.org/) as a scripting language for quickly writing tools, extractors, dumpers etc...
-   [Kaitai Struct](https://kaitai.io/) for defining the archive format from which kaitai struct will generate parsers for us.
-   [HxD](https://mh-nexus.de/en/downloads.php?product=HxD20) as a hexdump tool for looking at raw archive files.
-   [Cutter](https://github.com/radareorg/cutter/releases) as a free disassember tool for looking at raw executable files and trying to understand how given executable works with our archive files.

I will try to list the tools I will be using at the start of each post.
