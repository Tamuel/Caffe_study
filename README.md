# Caffe Study
Repository for studying Caffe deep learning framework.

## Prerequisite
* Visual studio 2017
* Cuda version 9.2
* cuDNN version 7.6.1
* python 3.5.x
  * numpy
* [Boost 1.65.1 msvc 14.0 x64](https://dl.bintray.com/boostorg/release/1.65.1/binaries/)
* [MSBuild 2015](https://www.microsoft.com/en-us/download/details.aspx?id=48159)
  
## How to build
* I will call root folder of this repository as **$CAFFE$**
1. First you have to install **Visual studio 2017 (Or higher)**
1. And then, install **Cuda version** 9.2 and **cuDNN** 7.6.1 **(Which compatiable with cuda version)**
1. You have to modify **./cmake/Cuda.cmake** to proper SM version of your GPU device. **(line 7 and 44)**
  
   ```
   7   set(Caffe_known_gpu_archs "30 35 50 60 61")
   44  set(__nvcc_out "6.1")
   ```
  
1. Install **python** with version 3.5.x **(Must!)** and numpy

    ```
    pip install numpy
    ```

1. Must add or check Path Variables of Cuda and python

1. Install **Boost 1.65.1 for msvc 14.0**

1. Install **MSBuild 2015**

1. At CMD (Command line) change folder to **$CAFFE$** and type like this to build Caffe for window

    ```
    ./scripts/build_win.cmd
    ```

1. Then, in **$CAFFE$** there are new folder **"build"**
1. Open **Caffe.sln** in **"build"** folder
1. Build all projects of solutions by **"Release" mode**

## References
* [Caffe tutorials](https://caffe.berkeleyvision.org/tutorial/)
* [Caffe in a Day Tutorial](https://docs.google.com/presentation/d/1HxGdeq8MPktHaPb-rlmYYQ723iWzq9ur6Gjo71YiG0Y/edit#slide=id.gc2fcdcce7_216_438)
* [Intel / TAU Summer Workshop on Deep Learning and Caffe](http://courses.cs.tau.ac.il/Caffe_workshop/Bootcamp/)
* [API Documentations](https://caffe.berkeleyvision.org/doxygen/annotated.html)
