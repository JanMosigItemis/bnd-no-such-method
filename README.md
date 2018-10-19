See https://github.com/bndtools/bnd/issues/2311

A test project to showcase an error when running JUnit based integration tests in an OSGi container with bnd.

* Have a copy of Eclipse 2018-09 (4.9.0) with bnd 4.0.0 ready.
* Open IDE with a new empty Eclipse workspace.
* Import the bnd workspace located in this repository.
* Right click on the `testproject` and choose Run -> Bnd OSGi Run Launcher (JUnit).
* java.lang.NoSuchMethodException: aQute.tester.plugin.ProjectTesterImpl.<init>(aQute.bnd.build.Project)
* The same problem will also appear if you try to compile this project on console.

## How to compile on console:

`./gradlew clean build`

