# jetson-yolo

jetson-yolo based on NVIDIA DeepStream 6.3

# Prerequisites

You must have the following development packages installed

    GStreamer-1.0
    GStreamer-1.0 Base Plugins
    GStreamer-1.0 gstrtspserver
    X11 client-side library
    Glib json library - json-glib-1.0
    yaml-cpp

To install these packages, execute the following command:

```
$ sudo apt-get install libgstreamer-plugins-base1.0-dev libgstreamer1.0-dev \
  libgstrtspserver-1.0-dev libx11-dev libjson-glib-dev libyaml-cpp-dev
```

# Compile

- For Jetson, CUDA_VER=11.4
- For x86, CUDA_VER=12.1

```
$ export CUDA_VER=XY.Z
$ make
```

# Usage

Run the application by executing the command:
```
$ ./jetson-yolo -c <config-file>
```