# HelloWorld

命令行编译opencv程序需要加参数: `pkg-config opencv --libs --cflags opencv`. 本例命令行编译执行:  

```shell
g++ hello_world_opencv.cpp `pkg-config opencv --libs --cflags opencv` -o hello_world

./hello_world
```

结果如下:  
![HelloWorld](/HelloWorld/HelloWorld.png) 

---

`namedWindow("Output",1);`  

![namedWindow](/HelloWorld/namedWindow.png)  

---

`Mat output = Mat::zeros( 120, 350, CV_8UC3 );`  

**Mat::zeros**  
![mat_zeros](/HelloWorld/mat_zeros.png)

**Mat::ones**  
Returns an array of all 1’s of the specified size and type.  

To fill a pre-existing Mat object with zeros, you can use Mat::zeros():  

``` c++
Mat m1 = ...;
m1 = Mat::zeros(1, 1, CV_64F);
```  

To intialize a Mat so that it contains only zeros, you can pass a scalar with value 0 to the constructor:  

``` c++
Mat m1 = Mat(1,1, CV_64F, 0.0);
```  

---

**putText**  
![putText](/HelloWorld/putText.png)  

Other [Drawing Function](https://docs.opencv.org/3.0-beta/modules/imgproc/doc/drawing_functions.html) like circle, ellipse etc.  

![drawingFunction](/HelloWorld/DarwingFunctions.png)

---

**imshow**  
![imshow](/HelloWorld/imshow.png)

---

**waitKey**  
![waitKey](/HelloWorld/waitKey.png)  

Zero means to wait forever.