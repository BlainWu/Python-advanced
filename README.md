# Python-advanced
总结一些高级的Python用法，知识点比较零散  
# 目录  
[1.属性和方法](##1.属性和方法)  
[2.抽象基类模块](##2.抽象基类模块)  
[3.有趣的\*args和**kwargs](##3.有趣的*args和**kwargs  )  
[4.修饰器](## 4.修饰器)

## 1.属性和方法  
1) @property修饰器，在类中可以将函数修饰为属性。这样在调用的时候，可以将函数当作属性来调用，不再需要括号和传参  
2) hasattr函数，判断对象是否有有一个方法或者属性  
3) getattr函数，获取一个方法或者属性  
4) setattr函数，设置一个方法或者属性(可选：如果没有则生成)  

## 2.抽象基类模块 ABC
**抽象类是一种特殊的类，这种类只能被继承，并且类中的抽象方法必须被实现。**  
比如，创建一个抽象的phone类。手机有各种品牌，但是没有叫手机的手机品牌。
同时，手机必须有屏幕，显示手机品牌（抽象方法）；但是不一定能连接5G信号（一般方法）。

## 3.有趣的\*args和**kwargs  
\*args和\*\*kwargs分别代表着arguments和keyword arguments，
当函数参数里包含他们的时候，函数参数的长度是可以变化的。
\*args用来保存tuple型的值，而\*\*kwargs用来保存保存字典类型的值。
值得一说的是，起作用的其实是\*号，而非args和kwargs，其他单词也可以。
\*和\*\*还可以用来解包数组和字典,对应固定的参数。  

## 4.修饰器  
修饰器可以简化在原有函数的基础上添加功能。  
这个示例从函数指针讲起，慢慢的到一个成熟的修饰器。  
还可以拓展的部分是：（1）加上\*args和\*\*kwargs （2）修饰函数还可以写成类的形式。
