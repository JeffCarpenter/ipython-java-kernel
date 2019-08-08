# 

# IPython Java Kernel
An IPython kernel for Java 9+.

## Expectation Setting
This is an experimental ipython kernel. Don't expect this to be production ready.

## Requirements

Install JDK 9+

This kernel expects two environment variables defined, which can be set in the kernel.json (described below):

## Installing the kernel

Assuming you have cloned the repo and got all the requirements above setup:

```python3 -m javakernel install --user```

If it worked you should be able to run the kernel:
```
[1] String a = "test"

|  Added variable a of type String with initial value "test"

```
