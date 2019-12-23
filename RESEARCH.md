## RESEARCH

### Troubleshooting
- `gtest_main` not found:  
  Download `libgtest-dev` package and build it.  
  And then copy the library or make an symbolic link so that autoreconf can find google test library.
- [javac] package does not exist:  
  Copy the compiled thrift java library to `lib/java/ directory`.  
  Then edit `Makefile.am` and `build.xml` files in the directory to replace `libthrift.jar` with the name of the copied .jar file.
- Could not create/open file:  
  Make a directory named `localfs` in the root directory.  
  Then grant write permissions to the group and others.
