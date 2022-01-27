Testing the Fac build system:

* Language-agnostic: Yes, seemingly

* No DSL: No - there is a small DSL for the language. New rules must start with "| ", dependencies with "<", and products with ">"

* Precise dependencies: No - Fac can miss dependencies if the user doesn't manually specify them and it may need to be run multiple times to fully determine dependencies

* General dependencies: No - directories are not always properly handled. Try building the current project multiple times (just type "fac" or "../fac/fac" if on Nikabrik) - the first build will correctly move the hello executable to the foo folder, but the second build will simply create a new hello executable in the cwd

* Automatic dependencies: Partially. The user can choose not to specify any dependencies, but the build may fail or do the wrong thing and require re-running Fac multiple times

* Dynamic incremental builds: Yes - using ptrace

* Automatic incremental builds: Partially. Again, the build may fail or do the wrong thing until Fac is run multiple times