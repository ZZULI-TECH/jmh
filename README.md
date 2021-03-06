# Code Tools: jmh
JMH is a Java harness for building, running, and analysing nano/micro/milli/macro benchmarks written in Java and other languages targetting the JVM.

# Basic Considerations
The recommended way to run a JMH benchmark is to use Maven to setup a standalone project that depends on the jar files of your application. This approach is preferred to ensure that the benchmarks are correctly initialized and produce reliable results. It is possible to run benchmarks from within an existing project, and even from within an IDE, however setup is more complex and the results are less reliable.

In all cases, the key to using JMH is enabling the annotation- or bytecode-processors to generate the synthetic benchmark code. Maven archetypes are the primary mechanism used to enable this. We strongly recommend new users make use of the archetype to setup the correct environment.
