# OPENCV-NOTES

## 命令行编译opencv

```shell
g++ main.cpp -o main `pkg-config --cflags --libs opencv`
```

## [查看opencv版本号](https://blog.csdn.net/lzh2912/article/details/52494891/)

```shell
pkg-config --modversion opencv
# 3.4.0
```