# 代码审查

## 看作业后的建议
* 选择合适的标签。选择某个标签的原因不能因为外观。比如为来实现几个元素在一行而选择用 td 标签；为了加粗而选择 strong 标签。
* 外观应该用 CSS 来做
  * 如段落缩进两个字，不应该用 &nbsp;&nbsp;。 应该用 `text-align: 2em`。
* 优化项
  * 给 a 加上 title 属性。
  * 给 img 加上 alt 属性。
  * 少用 id，多用 class。唯一的用id，一类东西用 class。 
  * 合适的命名。必要用 article1, article2 这种命名。
