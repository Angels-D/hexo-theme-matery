# hexo-theme-matery-s 主题

基于[hexo-theme-matery](https://github.com/blinkfox/hexo-theme-matery)主题做了一些修改，仿自[MX (mx142.cn)](https://mx142.cn/)

* 将功能集成到`_config.yml`中调用
* ~~修改css样式，去除部分冗余~~

[原版中文说明](README_CN.md) [Original README](README_EN.md)

## 详细内容

### 特效

* 鼠标点击
  * 新增或修改：修改
  * 文件位置：`/source/libs/others/clocklove.js` **»** `/source/js/click.js`
  * 内容：点击出现颜文字
* 加载动画
  * 新增或修改：新增
  * 文件位置：`/layout/_partial/loading-pages.ejs`
  * 内容：刷新页面加载动画（时钟 + 文字）
* 打字特效
  * 新增或修改：新增
  * 文件位置：
    * `/layout/_partial/typing_effect.ejs`
    * `/source/libs/others/activate-power-mode.min`
  * 内容：打字出现礼花和震动效果
* 标题变化
  * 新增或修改：新增
  * 文件位置：
    * `/layout/_partial/head.ejs` 第89-100行
  * 离开或进入页面时标题内容发生变化

### 排版

* 菜单栏
  * 新增或修改：修改
  * 内容：
    * 原`tages` `categories` `archives` 整合到`Essay`标签中
    * 原`contact` `friends` 整合到`Link`标签中

### 样式

* 导航栏/标签

  * 新增或修改：修改
  * 文件位置：`/source/css/matery.css` `bg-color`项
  * 内容：
    * 颜色改为渐变色
    * 透明效果
* 页脚黑色透明效果 `/source/css/matery.css` `footer`项
* 夜间模式按钮

  * 新增或修改：新增
  * 文件位置：`/layout/_widget/darkmode.ejs`
* 鼠标样式

  * 文件位置 `/source/medias/cursor`

  * 内容：
    * 新增更多样式
* 滑动条样式
  * 文件位置 `/source/css/matery.css`

### 内容

* 404页面
  * 新增或修改：新增
  * 文件位置：
    * `/layout/_games`
    * `/layout/404.ejs`
  * 内容：”围住猫“ 游戏
* 页脚
  * 新增或修改：新增
  * 文件位置：
    * `/layout/_partial/footer.ejs`
  * 内容：
    * 新增访客地图**clustrmaps**
    * 新增**github-badge**

### 修复

* valine

  > 新版valine需要指定服务端URL
