### 任务四：定位和居中问题
垂直，水平居中看下[任务提供的参考资料](http://ife.baidu.com/course/detail/id/95)
* 水平居中
  * 文本居中 `text-align:center`
  * 文档居中 
    * 处于文档流中：`margin:x auto`
    * 脱离文档流：绝对定位+margin负边距
* 垂直居中
  * 这里使用固定定位+margin负边距
* 圆角画法
  [参考:CSS3:border-radius隐藏的威力](http://www.xincss.com/?p=221)
* 参考资料，详细看任务后面的链接。举例如下，可能其他的没注意看到，有空再翻看看:
  * [清除浮动（clearfix hack）](http://zh.learnlayout.com/clearfix.html)
    * 这个例子使用`overflow:auto` 清除浮动，兼容ie。对比 `xxSel:after{content:'';visible:hidden;clear:both}`
  * [清除浮动黑科技完整解读](http://stackoverflow.com/questions/211383/which-method-of-clearfix-is-best)
