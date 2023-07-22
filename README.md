### 新的开始
### blog开通！！！

#### 1.在markdown中使用MathJax编写公式，却在HTML页面显示不了公式问题。

(1).在`layouts`中`post.html`加入以下代码。
```
<script src="mathjax-config.js" defer></script>
<script type="text/javascript" id="MathJax-script" async
 src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>
```
  (2).在js文件中加入`mathjax-config.js`文件，代码如下。
  ```
  window.MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']]
  },
  svg: {
    fontCache: 'global'
  }
};
```
[具体来源](https://zhuanlan.zhihu.com/p/165963112)

