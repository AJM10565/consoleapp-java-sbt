[![Build Status](https://travis-ci.org/LoyolaChicagoCode/hello-java-sbt.svg?branch=master)](https://travis-ci.org/LoyolaChicagoCode/hello-java-sbt)

This build will always fail because it has 2 examples of failing tests:
one because of a defect in the SUT (system under test), and one because of an error in the test itself.

# Learning Objectives

* Simple hello world example
* Experience with Git source code management
* Building with SBT
* Automated unit testing with JUnit
* Continuous integration with Travis

# System requirements

* Java 8 SDK or later
* [SBT](https://www.scala-sbt.org/1.x/docs/Setup.html)

# Running the Application

On Linux or Mac OS X:

    $ sbt run

or

    $ sbt 'run arg1 arg2 arg3'
	
On Windows:
	
    > sbt run

or

    > sbt "run arg1 arg2 arg3"

# Running the Tests

On Linux or Mac OS X:

    $ sbt test
	
On Windows:
	
    > sbt test

# Running the Application Outside SBT

This allows passing command-line arguments directly:

On Linux or Mac OS X:

    $ sbt stage
    $ ./target/universal/stage/bin/hello-java arg1 arg2 arg3

On Windows:

    > sbt stage
    > .\target\universal\stage\bin\hello-java arg1 arg2 arg3
