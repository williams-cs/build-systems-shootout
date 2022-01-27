Testing the Stroll build system:

* Language-agnostic: Yes, seemingly

* No DSL: Yes - build files can be written in your language of choice

* Precise dependencies: Unsure - needs testing

* General dependencies: No - antidependencies are not supported (stated in documentation)

* Automatic dependencies: Yes

* Dynamic incremental builds: Yes - using fsatrace

* Automatic incremental builds: Unsure - also needs testing. fsatrace was having issues when I tried to build the current project but I'm uncertain what the problem was