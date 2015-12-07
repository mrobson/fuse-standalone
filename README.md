# fuse-fabric8-docker

fuse-base-openjdk7
------------------
Base level image, installs JDK7 and sets JAVA_HOME.

fuse-base-openjdk8
------------------
Base level image, installs JDK8 and sets JAVA_HOME.

fuse-base-os
------------
Base OS, builds on the base JDK image.  Adds users, directories, OS level tuning and parameters.

fuse-base-install
-----------------
Base Fuse binary installation, builds on the base OS image.  Adds Fuse specific environment variables, downloads the Fuse artifact, installs the binary, cleans up redundant files, edits common Fuse configurations, sets up standard out logging for docker and some default JVM options.

fuse-standalone
---------------
Base image for a running Fuse standalone container, builds on the base Fuse install.  This image sets the correct user (this is more so for posterity and read ability), exposes the necessary ports, sets working directories, sets the entry point and the start up commands.

