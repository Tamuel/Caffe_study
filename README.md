# Caffe Study
Repository for studying Caffe deep learning framework.

## Prerequisite
* Visual studio 2015
* Cuda version 8.0
* cuDNN version 7.1.3
* python 3.5.x
  * numpy
  
## How to build
* I will call root folder of this repository as $CAFFE$
1. First you have to install Visual studio 2015
2. And then, install Cuda version 8.0 and cuDNN 7.1.3 (Which compatiable with cuda version)
3. Install python with version 3.5.x (Must!) and numpy

```
pip install numpy
```

4. Must add or check Path Variables of Cuda and python

5. At CMD (Command line) change folder to $CAFFE$ and type like this to build Caffe for window

```
./scripts/build_win.cmd
```

6. Then, in $CAFFE$ there are new folder "build"
7. Open Caffe.sln in "build" folder
8. Build all projects of solutions by "Release" mode

