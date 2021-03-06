### 更新日志

2018.10.28

-   编写 2.0 版本，添加裁剪区域宽度高度比例的控制，而不是以往的 750 \* 750 而导致页面显示的内容不充分的视觉效果（通过 CROPPER_RATIO 来控制 cropper 的宽高比例 默认是 0.6666 接近于宽 640 / 高 960）
-   添加固定比例裁剪功能 CROPPER_AREA_RATIO 在设置为 > 0 的 number 值的时候可以控制裁剪的比例，比例也是宽高的比，如果是正方形则为 1，如果不想有比例的裁剪，这个常量设置为 0 即可
-   优化界面 UI
-   这些代码还有部分问题，暂时没有放到 master，有需要或者了解的可在[v2](https://github.com/IFmiss/wx-cropper/tree/v2)分支拉取代码

    2018.8.16

-   代码重写，裁剪机制变化
-   修复安卓机裁剪时卡顿的问题
-   修复裁剪边框超出的问题

    2018.4.23

-   新增图片质量控制，参数为 qualityWidth，避免图片过大时导致内存溢出
-   新增本地图片上传裁剪功能

# wx-cropper

微信小程序 图片裁剪工具，简单易用

QQ 交流群： 424418160

### 项目需求

在做微信小程序的时候有个图片上传之前裁剪的需求，找过一些 github 中的项目，都不太理想，主要是没有办法自定义宽高，于是自己研究了一下，做了一个简单的图片裁剪效果

### 使用方法

项目里面直接放的该功能的文件，将这个文件夹复制到小程序项目中，在 app.json 中启动该页面即可看到效果

### 注意：这里面的图片在你们的项目中可能会无法使用，在测试的话 可以用自己本地或者你们项目服务器下的图片地址

### 显示效果

#### 裁剪之前的效果

![](https://github.com/IFmiss/wx-cropper/blob/master/1.png)

#### 裁剪之后的效果

![](https://github.com/IFmiss/wx-cropper/blob/master/2.png)

## 感谢大佬的插件

由于自己的项目用的 mpvue 框架，于是把小程序组件翻译成 vue 组件了。一字未改，原版翻译。
