# icon-font图标字体

>有一个岗位，叫`前端开发`；有一种技术，叫 `CSS Sprite`；有一种突破，叫`font+HTML/CSS`。

移动互联网时代的到来，让CSS Sprite似乎有点Hold不住。Font+HTML/CSS将会做到，小巧的体积、更快的加载速度、任意改变颜色和尺寸，完美的兼容性，是你在网页中画小图标的不二之选。

在过去，我们为了使网页变得丰富多彩，免不了会使用一些小按钮、小图标，相信聪明的你对CSS Sprites（CSS精灵）一点也不陌生。
那么，现在呢？如果你只知道CSS Sprites，那么你就有点OUT了。今天要给大家介绍的是一种更方便、高效，在多种设备上完美显呈现的小图标技术。[http://www.flowerboys.cn/font](http://www.flowerboys.cn/font)

### 课程简介:
> 你有想过在网页中画小按钮、小图标就像在网页中输入文本一样高效、快捷吗？
> * 是的，她将成为现实。她在天猫、淘宝、土豆、优酷等国内大型网站上已经开始崭露头角。她绝对是前端开发里的一场盛宴。可以通过font-size来改变图标大小，通过color改变颜色等；她体格娇小，兼容所有主流浏览器，并且在所有现代浏览器里实现放大、旋转等CSS3动画效果效果。
>* 在各种分辨率下她都能高清无码完美显示展现自己迷人的风采，她绝对会令你大开眼界，你一定会深深的爱上她。

### 你能学到什么？
>* eot、woff、ttf、svg字体格式
>* `@font-face`、font-family字体相关属性
>* `:before`、`:after`伪元素，`content`属性
>* 使用 [IcoMoon App](https://icomoon.io) 管理字体图标
>* 轻松改变图标大小及颜色等CSS属性，就像`操作文本`一样简单。

## 代码演示
下面我们来展示两种用字体在网页中画小图标的方法：
![show](source/show.jpg)

### 一、HTML实体
* HTML结构部分
```html
<i class="icon-ui">&#xe600;</i>
<i class="icon-ui">&#xe601;</i>
<i class="icon-ui">&#xe602;</i>
<i class="icon-ui">&#xe603;</i>
<i class="icon-ui">&#xe604;</i>
```

* CSS样式部分
```css
@font-face {
  font-family: 'icon-font';
  src:url('fonts/icomoon.eot');
  src:url('fonts/icomoon.eot?#iefix') format('embedded-opentype'),
      url('fonts/icomoon.ttf') format('truetype'),
      url('fonts/icomoon.woff') format('woff'),
      url('fonts/icomoon.svg') format('svg');
  font-weight: normal;
  font-style: normal;
}

.icon-ui {
  font-family: 'icon-font';
  speak: none;
  font-style: normal;
  font-weight: normal;
  font-variant: normal;
  text-transform: none;
  line-height: 1;
  /* Better Font Rendering =========== */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
```

### 二、class名称
* HTML结构部分
```html
<i class="icon-chrome"> </i>
<i class="icon-firefox"> </i>
<i class="icon-IE"> </i>
<i class="icon-opera"> </i>
<i class="icon-safari"> </i>
```

* CSS样式部分
```css
@font-face {
  font-family: 'icon-font';
  src:url('fonts/icomoon.eot');
  src:url('fonts/icomoon.eot?#iefix') format('embedded-opentype'),
      url('fonts/icomoon.ttf') format('truetype'),
      url('fonts/icomoon.woff') format('woff'),
      url('fonts/icomoon.svg') format('svg');
  font-weight: normal;
  font-style: normal;
}

[class^="icon-"], [class*=" icon-"] {
  font-family: 'icon-font';
  speak: none;
  font-style: normal;
  font-weight: normal;
  font-variant: normal;
  text-transform: none;
  line-height: 1;
  /* Better Font Rendering =========== */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.icon-chrome:before  { content: "\e600"; }
.icon-firefox:before { content: "\e601"; }
.icon-IE:before      { content: "\e602"; }
.icon-opera:before   { content: "\e603"; }
.icon-safari:before  { content: "\e604"; }
```

## 视频教程 
《[用字体在网页中画Icon小图标](http://www.imooc.com/view/243)》

## 总结
这里我们介绍了两种使用字体在网页中画小图标的技巧：
* 第一种方法 《HTML实体》可以完美兼容到糟糕的IE6，完全有理由放心、大胆的使用。
* 第二种方法 《class名称》它没有第一种那么繁琐，如果您的项目中不需要考虑糟糕的IE7-，那么使用本方法简直了。

***

## 说明
* 营销官网：`http://www.threetowns.cn`
* 技术支持：`http://www.flowerboys.cn`

## 技术支持
>[三镇网络技术有限公司](http://www.threetowns.cn)，专注于网络营销、电子商务和企业定制化建站服务，把正确的营销方向当作一种使命，帮助客户提供专业的网络营销方案。其雄厚的实力，专业的营销团队一直活跃于各大电子商务平台的前线。

## 联系方式

* EMAIL联系方式：`threetowns@163.com`

| 官方网站 | 技术微信 | 技术QQ | QQ交流群 |
|--------|--------|--------|--------|
|![qq-1209445709](https://github.com/threetowns/About/raw/master/qrCode/website_threetowns.cn.jpg)|![wechat-433238694](https://github.com/threetowns/About/raw/master/qrCode/wechat_yonger_lei.jpg)|   ![qq-1209445709](https://github.com/threetowns/About/raw/master/qrCode/qq_1209445709.jpg)     |    ![qq-433238694](https://github.com/threetowns/About/raw/master/qrCode/qqGroup_433238694.jpg)    |
