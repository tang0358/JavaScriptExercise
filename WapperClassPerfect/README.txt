完美版的封装class类名

1.因为一个元素标签可能同时出现多个类名，比如：
		<div class="demo test"></div>
这个时候我们采用上一个demo中使用的遍历所有元素之后，得到的类名就会是"demo test",和"demo"不相等因而错过了这个div,造成了误差

2.我们将"demo test"用split方法分割转换成数组，["demo","test"]然后遍历这个数组；如果遍历到有元素和"demo"相等，则把对应的div用Push方法推入数组末端；最后得到我们想要的div的伪数组集合

3.可以作为外联js文件的初始程序，处理浏览器对于className的兼容问题