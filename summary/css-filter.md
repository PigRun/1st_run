# 神奇的滤镜

相信大家都熟悉各类图片应用中提供的那些魔法般的滤镜效果。原本这些滤镜最初都大量的用于SVG中，随着浏览器的不断发现，Web标准的更新，这个特性被W3C引入CSS中，同时针对这一特性还制定了相关的[标准规范](https://dvcs.w3.org/hg/FXTF/raw-file/tip/filters/index.html)。

下面就跟随我们一起来探索以下这个神奇的魔法吧。

一个示例效果：

![filter](src/filter.gif)

没错，这些浏览器中的效果都是用CSS实现的。率先实现这一特性的`webkit`内核的浏览器实现了规范中以下效果：

- grayscale 灰度
- sepia 褐色
- saturate 饱和度
- hue-rotate 色相旋转
- invert 反色
- opacity 透明度
- brightness 亮度
- contrast 对比度
- blur 模糊
- drop-shadow 阴影

而实现这些效果只编写标准少量标准的CSS语法即可：

```css
-webkit-filter: <effectOptions>
```

现在，这些原本需要我们动手懂各种图片软件处理的效果，用CSS也能实现。并且效果并不亚于使用这些图片处理软件的实现。

下面是一些国内外工程师们实现的效果演示：

- [CSS3滤镜效果演示](http://labs.qianduan.net/css_filter.html)