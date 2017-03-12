# 代码审查

## 看作业后的建议
* 选择合适的标签。选择某个标签的原因不能因为外观。比如不能为了实现几个元素在一行而选择用 td 标签；为了加粗而选择 strong 标签。
* 外观应该用 CSS 来做。如段落缩进两个字，不应该用 &nbsp;&nbsp;。 应该用 `text-align: 2em`。
* 减少不必要的标签
  * 导航li的点，你是用一个空的b标签来实现的。li本身就带点的。如果一定要自己画那个点，更好的方式是用伪类选择器 :before 来做。
* 优化项
  * 给 a 加上 title 属性。
  * 给 img 加上 alt 属性。
  * 少用 id，多用 class。唯一的用id，类似的用 class。 
  * 合适的命名。不要用 article1, article2 这种命名。如果 article1 和 article2 是大部分外观是类似的，给他们加上 article 的类名。再给他们加上不同的类名来定义不同的外观，如 article--small, article--primary 之类的。
