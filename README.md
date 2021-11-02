# fprime-python-examples

If you don't know what this is, start with: [fprime-python](https://github.com/LeStarch/fprime-python). This example
takes the `SignalGen` component and implements it in Python. There are four key files to reference:

1. PyApp/SignalGen/SignalGen.py: an implementation of the component in Python!
2. PyApp/SignalGen/CMakeLists.txt: the `CMakeLists.txt` for integrating a component with fprime-python bindings
3. PyApp/CMakeLists.txt: the `CMakeLists.txt` deployment setup for running fprime-python applications
4. PyApp/Top/Main.cpp: the main file including the initialization for fprime-python

## Setup This Example

In order to setup this example, run the following commands. 

```bash
git clone https://github.com/LeStarch/fprime-python-examples.git
cd fprime-python-examples/
git submodule update --init --recursive
```

## Building This Example

To run, follow the standard generate and build steps for fprime deployments.  The deployment is in the PyApp folder.

```bash
cd PyApp
fprime-util generate
fprime-util build
```

## Running This Example

Running this example should be easy as long as PYTHONPATH is set. Python files end up in the `build-artifacts/python`
and thus this folder must be on the PYTHONPATH when running.

```bash

```
