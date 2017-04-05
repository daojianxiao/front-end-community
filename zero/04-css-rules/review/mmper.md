# mmper
1. 作业1 [源码](https://github.com/mmper/front-end-demos/blob/master/04-css-rules/demo.html)
1. 作业2 [文章:背景定位&背景尺寸](http://www.jianshu.com/p/9452493b856e)

作业1:建议
1 选择合适的标签。如`<p>ife.baidu.com</p>` 应该用标签 h1。  
2 将布局的 CSS 写成一个文件，方便以后复用。如，头部的HTML这么写
```
<header id="top" class="ly ly--justify">
  <h1 class="ly__item">ife.baidu.com</h1>
  <span class="ly__item">2016.3</span>
</header>
```
CSS
```
.ly:before{
    content:"";
    display: table;
}
.ly:after{
    content:"";
    display:block;
    clear: both;
}
.ly__item{
  float: left;
}
/* ly--justify 表示两端对齐 */
.ly--justify .ly__item:last-child{
  float: right;
}
```
用float布局就是不灵活啊，可以参考我写的布局的CSS，点[这里](https://github.com/iamjoel/baidu-ife-task/blob/master/src/2017/lib/layout.css)。

