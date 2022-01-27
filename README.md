# build-systems-shootout
A repository of build systems, including examples showing whether a given system satisfies certain properties

These properties are:

* Language-agnostic: can you build programs in any language with this system?

* No DSL: is there a programming language specifically designed for the system?

* Precise dependencies: does the system guarantee that all dependencies are always captured? 

* General dependencies: does the system support cyclic dependencies, antidependencies, and non-file objects?

* Automatic dependencies: can the system automatically determine dependencies without the user manually specifying them?

* Dynamic incremental builds: can the system discover dependencies at build time?

* Automatic incremental builds: can the system discover dependencies at build time without the user providing any sort of helper functions or hooks in their code?

The Excel sheet in this repository provides a starting point for assessing a variety of build systems for these properties. 
