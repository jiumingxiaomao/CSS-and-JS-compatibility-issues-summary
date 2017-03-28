# CSS-and-JS-compatibility-issues-summary（CSS和JS兼容性问题总结）

是时候该总结一下自己工作以来遇到的css和js的兼容性问题了。

## CSS兼容性问题

## JS兼容性问题
* 判断数据类型

## 移动端兼容性问题（H5兼容性问题）
* 父元素使用了transform，子元素position:fixed失效的问题

我的页面中有个这样的需求，点击定位，页面从右向左拉出一个菜单，覆盖整个屏幕，这个滑动效果我是用transform写的，可以选择省，但是上面当前位置和取消所占的一行要求position:fixed，下面的省可以滚动，效果如下图：

![](https://github.com/FloweringVivian/CSS-and-JS-compatibility-issues-summary/blob/master/images/img1.jpg)  

结果就是position:fixed失效了，因为他的父元素运用了transform，我的解决办法就是改变布局，让需要position:fixed的元素变成transform元素的兄弟元素，而不是子元素，这样就解决了，如果有更好的解决办法，欢迎大家踊跃发言告知，在此感谢！
