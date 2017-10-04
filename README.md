# 

# java9_kernel
An ipython kernel for java 9. Last tested Kulla.jar was kulla--20160821005845.jar

## Expectation Setting
This is an experimental ipython kernel written with an experimental repl written for
a unreleased java version. Don't expect this to be production ready.

That being said. File issues and I'll do my best.

## Requirements

Install [java9-openjdk]

This kernel expects two environment variables defined, which can be set in the kernel.json (described below):

```
JAVA_9_HOME - like JAVA_HOME but pointing to a java 9 environment
```

## Installing the kernel

Assuming you have cloned the repo and got all the requirements above setup

edit kernel.json replacing PATH_TO_javakernel to the location of the javakernel directory
 
```
mkdir ~/.ipython/kernels/java/

cp <location of your edited kernel.json> ~/.ipython/kernels/java/
```

For example a kernel.json might look like this:

```
{
 "argv": ["python3", "<javakernel_path>",
          "-f", "{connection_file}"],
 "display_name": "Java 9",
 "language": "java",
 "env" : {
     "JAVA_9_HOME": "<java_path>",
     }
 }       
```

If all worked you should be able to run the kernel:
```
[1] String a = "test"

|  Added variable a of type String with initial value "test"

```
