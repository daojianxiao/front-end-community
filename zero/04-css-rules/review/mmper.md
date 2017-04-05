# mmper
1. 作业1 [源码](https://github.com/mmper/front-end-demos/blob/master/04-css-rules/demo.html)
1. 作业2 [文章:背景定位&背景尺寸](http://www.jianshu.com/p/9452493b856e)

作业1:建议  
1 选择合适的标签。如`<p>ife.baidu.com</p>` 应该用标签 h1。About 和 TECHNOLOGE 不应该用 h1 标签。 `<a>前</a>` 这标签用的也不对。  
2 将布局的 CSS 写成一个文件，方便以后复用。如，头部的HTML这么写  
```
<header id="top" class="ly ly--justify">
  <h1 class="ly__item">ife.baidu.com</h1>
  <span class="ly__item">2016.3</span>
</header>
```
CSS 这么写  
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

3 类似的东西用一个类名，而不是不同的类名。如 what，when， how。HTML 可能是这么写
```
<div class="panel panle--what">
  <h3>What</h3>
  <article>....</article>
</div>
<div class="panel panle--when">
  <h3>when</h3>
  <article>....</article>
</div>
<div class="panel panle--how">
  <h3>how</h3>
  <article>....</article>
</div>
```

4 尽量不要用标签选择器，用类名。  
5 选择器尽量不要超过2级，不要出现这种 `.bottom-rt div>p`， `.bottom-rt div>p span`这种。解决方式还是通过类名。

总而言之，功能是实现了，写了很多脆弱的选择器，需要加强。我晚点写篇文章介绍下如何写选择器。

作业2:  
归纳整理的很赞~


