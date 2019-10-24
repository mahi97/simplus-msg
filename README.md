# simplus-msg


## Setup

### Prerequisites

gRPC Python is supported for use with Python 2.7 or Python 3.4 or higher.
Ensure you have pip version 9.0.1 or higher:
```bash
$ python -m pip install --upgrade pip
```

If you cannot upgrade pip due to a system-owned installation, you can run the example in a virtualenv:

```bash
$ python -m pip install virtualenv
$ virtualenv venv
$ source venv/bin/activate
$ python -m pip install --upgrade pip
```
### Install gRPC
```bash
$ python -m pip install grpcio
```
Or, to install it system wide:
```bash
$ sudo python -m pip install grpcio
```
On El Capitan OSX, you may get the following error:
```bash
$ OSError: [Errno 1] Operation not permitted: '/tmp/pip-qwTLbI-uninstall/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/six-1.4.1-py2.7.egg-info'
```
You can work around this using:
```bash
$ python -m pip install grpcio --ignore-installed
```
### Install gRPC tools (to re-write the messages) 

Python’s gRPC tools include the protocol buffer compiler protoc and the special plugin for generating server and client code from .proto service definitions. For the first part of our quickstart example, we’ve already generated the server and client stubs from helloworld.proto, but you’ll need the tools for the rest of our quickstart, as well as later tutorials and your own projects.

To install gRPC tools, run:
```bash
$ python -m pip install grpcio-tools
```


### Run 

Run the server:
```bash
  python3.5 server.py
```

Run the client:
```bash
  python3.5 client.py
```
