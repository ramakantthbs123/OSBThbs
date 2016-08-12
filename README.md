Maven OSBSample build
===================================================================

main pom ( /pom.xml ) which build the OSBSample
 
Important
---------
with java as goal for the exec-maven-plugin does not seems to work because you are running inside 
the maven jvm ( no fork ) and need to set MAVEN_OPTS parameters to pass on -D parameters but all this
Also adding dependecies libraries and using includeProjectDependencies does also work.

need to use exec as goal to start a new process and use commandlineArgs, you can't use arguments
