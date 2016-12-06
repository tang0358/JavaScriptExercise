1.封装自己的class类名的原因：
访问DOM的方法中，getElementByClassName并不适用于低版本的IE5,6,7,8浏览器；所以若想使得有className的元素也可以被访问，必须封装自己的class类名。

2.对于高版本的浏览器：
if(document.getElementByClassName) //证明浏览器是否支持
 {
    return document.getElementByClassName(classname); //返回一个伪数组
 }

3.对于低版本不支持className 的浏览器:
我们要取出所有的盒子， 利用遍历的方法 ， 通过每一个盒子的className 来判断。如果相等就留下。

4.这种写法并不完美：当一个标签含有多个类名时，就检测不出来了

