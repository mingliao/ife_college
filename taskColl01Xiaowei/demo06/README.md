* 浮动设置
  * #banner区域布局，把需要浮动的元素放到不浮动的元素前面。让它先浮动。再设置不浮动的元素，这样不浮动的元素依然在文档流中。浮动元素和不浮动元素就处于同一个水平位置了。这种方式可以参考任务03的浮动布局。
* 字体设置
  * 文本大小跟以下设置有关
   * fontsize有关，
     * 通过ps的文本划线查看大小，而不是通过查看文本的高度决定的。
   * 字体有关。
     * 有的字体比较胖，看起来字就比较大。
* 段落
  * 行高确定参考![ps确定](./img/line-height.png)
  * 段落因为有行高的关系，所以，要确定整个p标签的高度，必须把行高考虑在内。
    整个p的高度是文本的高度+(一个行高-文本fontsize，就是把文本高度上下补齐了。)
    ![ps确定](./img/p-height.png)
* ul设置
  * 如何确定与上面p段落的margin-top的值，参考段落的css设置判断p的实际高度。
    确定行高
  * li之间使用*margin-top*，还是*margin-bottom*
    * 使用margin-top，因为ul的margin-top和li的margin-top重叠，会叠加。
      使用上没什么障碍
      ![ul margin-top](./img/ul-height.png)
      ```
	      #article_cont ul {margin-top: 15px;list-style-type: none;} 

	      #article_cont li {font: 12px "微软雅黑";margin-top: 10px;}

	      #article_cont li span {color: #cd4a48;}
      ```
    * 使用*margin-bottom*，注意文本自己会把li撑开，所以要设置`line-height`使文本居中。
		![ul margin-top](./img/ul-height-margin-bottom.png)
      ```
		#article_cont ul {margin-top: 25px;list-style-type: none;}

		#article_cont li {font: 12px "微软雅黑";line-height: 12px;  margin-bottom:  8px;}

		#article_cont li span {color: #cd4a48;}
      ```