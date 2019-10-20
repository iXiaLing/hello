# Demo

## 链接 Demo
### 内嵌式连接
- 外部链接

	[百度](https://www.baidu.com)
- 内部链接相对引用

	[README](README.MD)
	
	[同级目录](./README.MD)
	
	[上级目录](../demo/abc.txt)
	
	[根目录](/RootDemo/root.txt)
	
	[文档内部跳转](#代码块-Demo)
- 内部链接绝对引用
	
	[绝对路径](C:\Users\Admin\Desktop\Test\hello\README.md)
	
### 引用式链接
-	[淘宝]
	
-	[阿里巴巴][alibaba]
	
-	I get 10 times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].
	
-	[本地文件][abc]

-	[代码块][Code Sample]
	
	<!--下面是本文需要用到的引用式链接，前面不能有空格--> 
[淘宝]: https://www.taobao.com
[alibaba]: http://1688.com/
[1]: http://google.com/        "Google" 
[2]: http://search.yahoo.com/  "Yahoo Search" 
[3]: http://search.msn.com/    "MSN Search"
[abc]: ../demo/abc.txt
[Code Sample]: #代码块-Demo
[Baidu Log]: https://www.baidu.com/img/bd_logo1.png?where=super

## 图片 Demo
![图片无法正常显示](images/Baidu.png)
![图片无法正常显示](https://www.baidu.com/img/bd_logo1.png?where=super)
![图片无法正常显示](https://www.baidu.com/img/bd_logo1.png?where=super "百度网站")
![图片无法正常显示][Baidu Log]


## 引用 Demo
>这是一段引用

----出自《xxx》

>>>一楼

>>二楼

>三楼


## 代码块 Demo
- 行内代码
	python示例代码`print("Hello World")`呵呵呵
	
- 块式代码
```python
	print("Hello World")
```

    print("Hello World")
	print("Hello World")