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
1. First you have to install Visual studio 2017
2. And then, install Cuda version 9.2 and cuDNN 7.6.1 (Which compatiable with cuda version)
3. Install python with version 3.5.x (Must!) and numpy

```
pip install numpy
```

4. Must add or check Path Variables of Cuda and python

5. Install **Boost 1.65.1 for msvc 14.0**

6. Install **MSBuild 2015**

7. At CMD (Command line) change folder to **$CAFFE$** and type like this to build Caffe for window

```
./scripts/build_win.cmd
```

8. Then, in **$CAFFE$** there are new folder "build"
9. Open Caffe.sln in "build" folder
10. Build all projects of solutions by "Release" mode

## References
* [Caffe tutorials](https://caffe.berkeleyvision.org/tutorial/)
* [Caffe in a Day Tutorial](https://docs.google.com/presentation/d/1HxGdeq8MPktHaPb-rlmYYQ723iWzq9ur6Gjo71YiG0Y/edit#slide=id.gc2fcdcce7_216_438)
* [Intel / TAU Summer Workshop on Deep Learning and Caffe](http://courses.cs.tau.ac.il/Caffe_workshop/Bootcamp/)
* [API Documentations](https://caffe.berkeleyvision.org/doxygen/annotated.html)
