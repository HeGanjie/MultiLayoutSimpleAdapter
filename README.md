MultiLayoutSimpleAdapter
========================

使得ListView能够呈现多种布局的多布局适配器 [浏览源代码](/MultiLayoutSimpleAdapter.java)

ListView用了SimpleAdapter之后就只能呈现一种Layout，这样虽然简单但是有时不能满足需求。所以，我下载了 **Android SDK 2.3.3** 的源码并修改了 **SimpleAdapter.java**。

各位下载了之后能将它当成SimpleAdapter使用。  

主要修改的地方是：  
1、构造方法不再接受单个Layout Resource，能接受**Resource数组**。  
2、能够根据 ItemViewType来选择Resource，所以子类应该要重写 `getItemViewType`。

### 图例，下面的控件均在同一个ListView内：
![例子](http://static.oschina.net/uploads/code/201301/18001622_RtwX.png "三种自定义布局")
