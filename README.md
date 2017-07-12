# Spriting with Compass
>Spriting has never been easier than it is with Compass. You place the sprite images in a folder, import them into your stylesheet, and then you can use the sprite in your selectors in one of several convenient ways.

![compass](http://riny.net/img/2014/compass.png)

## Getting started
* Install compass
 ```bash
 # 1. check ruby and sass
 $ ruby -v
 ruby 2.3.3p222 (2016-11-21 revision 56859) [x64-mingw32]

 $ sass -v
 Sass 3.4.23 (Selective Steve)

 # 2. install compass
 $ gem install compass

 # 3. check compass
 $ compass -v
 Compass 1.0.3 (Polaris)
 Copyright (c) 2008-2017 Chris Eppstein
 Released under the MIT License.
 Compass is charityware.
 Please make a tax deductable donation for a worthy cause: http://umdf.org/compass
```

* Init compass project
```bash
$ cd your-project
$ compass init
$ tree
 
 # your dirctory
├── config.rb
├── sass
│   ├── ie.scss
│   ├── print.scss
│   └── screen.scss
├── stylesheets
│   ├── ie.css
│   ├── print.css
│   └── screen.css
├── images            # Create new folder
└── .sass-cache
```

## 基础应用
* 开始之前，需要完成两步操作:`gem install compass`、`compass init`
* 在`sass`文件夹下，新建一个`<map>.scss`文件，代码如下：
```scss
@import "compass/utilities/sprites";
@import "colorful/*.png";                // <map>/*.png
@include all-colorful-sprites;           // all-<map>-sprites
```
* 在项目根目录，新建`images`文件夹。【见：`config.rb`的`images_dir = "images"`】
* 在`images`文件夹下，新建一个`<map>`文件夹，把我们需要合并的`png`图片放到该文件夹下
* 执行以下命令,进行编译
```bash
compass compile
```

## 高级应用-配置
```scss
@import "compass/utilities/sprites";
@import "colorful/*.png";                // <map>/*.png
@include all-colorful-sprites;           // all-<map>-sprites

$colorful-spacing: 5px;                  // 配置间距,<map>-spacing

//$colorful-position: 5px;               // 配置位置,<map>-position

// 参数：vertical/horizontal/diagonal/smart
$colorful-layout: vertical;              // 配置布局方式，<map>-layout

$colorful-sprite-dimensions: true;       // 自动输出尺寸，<map>-sprite-dimensions
```


## 说明
* 营销官网：`http://www.threetowns.cn`
* 技术支持：`http://www.flowerboys.cn`

## 技术支持
>[三镇网络技术有限公司](http://www.threetowns.cn)，专注于网络营销、电子商务和企业定制化建站服务，把正确的营销方向当作一种使命，帮助客户提供专业的网络营销方案。其雄厚的实力，专业的营销团队一直活跃于各大电子商务平台的前线。

***

## 联系方式

* EMAIL联系方式：`threetowns@163.com`

| 官方网站 | 技术微信 | 技术QQ | QQ交流群 |
|--------|--------|--------|--------|
|![qq-1209445709](https://github.com/threetowns/About/raw/master/qrCode/website_threetowns.cn.jpg)|![wechat-433238694](https://github.com/threetowns/About/raw/master/qrCode/wechat_yonger_lei.jpg)|   ![qq-1209445709](https://github.com/threetowns/About/raw/master/qrCode/qq_1209445709.jpg)     |    ![qq-433238694](https://github.com/threetowns/About/raw/master/qrCode/qqGroup_433238694.jpg)    |
