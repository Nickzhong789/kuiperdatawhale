# kuiperdatawhale


[https://github.com/zjhellofss/KuiperInfer](https://github.com/zjhellofss/KuiperInfer) ，欢迎大家点赞和PR.

# 环境安装

## Google系列

googletest

```bash
git clone https://github.com/google/googletest.git
mkdir build && cd build
cmake -Dgtest_build_tests=on -DCMAKE_INSTALL_PREFIX=. ..
make -j8
make install
cd include
cp -r gtest /usr/local/include
cp -r gmock /usr/local/include
```

googlebenchmark

```bash
git clone https://github.com/google/benchmark.git
cd benchmark
mkdir buil && cd build
cmake -DBENCHMARK_DOWNLOAD_DEPENDENCIES=on -DCMAKE_BUILD_TYPE=Release ..
make -j8
make install
```

glog

```bash
git clone https://github.com/google/glog
cd glog
mkdir build && cd build
cmake -DGFLAGS_NAMESPACE=google -DCMAKE_CXX_FLAGS=-fPIC -DBUILD_SHARED_LIBS=ON ..
make -j8
make install
```

Armadillo

```bash
apt-get install libarmadillo-dev -y
```

gtest

```bash
apt-get install libgtest-dev -y
```

## OpenCV

源码安装

```bash
git clone https://github.com/opencv/opencv.git
cd opencv
git checkout 4.x
mkdir build
cd build
mkdir -p /usr/local/opencv4.x
cmake -D CMAKE_BUILD_TYPE=Release -D CMAKE_INSTALL_PREFIX=/usr/local/opencv4.x ..
make -j8
make install
```


