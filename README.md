# 

# IPython Java Kernel
An IPython kernel for Java 9+.

## Expectation Setting
This is an experimental ipython kernel. Don't expect this to be production ready.

## Requirements

Install JDK 9+

This kernel expects two environment variables defined, which can be set in the kernel.json (described below):

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
 "display_name": "Java",
 "language": "java",
 "env" : {
     "JAVA_HOME": "<java_path>",
     }
 }       
```

If all worked you should be able to run the kernel:
```
[1] String a = "test"

|  Added variable a of type String with initial value "test"

```
