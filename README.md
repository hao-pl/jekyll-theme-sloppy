# Jekyll-theme-sloppy

一个基于Jekyll的blog主题Sloppy，本人初次使用github，正在努力学习如何使用。对于其中的问题希望各位积极指出，在下会尽快改正。多谢！:laughing:

## 主题简介

本主题为基于jekyll主题[Hyg](https://gaohaoyang.github.io/)做的个性化修改后的版本。感谢原作者的付出。

## 功能介绍

- [x] 增加图片大小和位置调节
- [x] 增加文字位置调节
- [x] 增加视频播放和音频播放功能
- [x] 支持内嵌引用Youtube、Bilibili、Ted等音频与视频
- [x] 去掉评论功能和google analysis等搜索计数功能
- [x]  优化显示效果，针对移动端进行优化
- [x] 重新对网页元素的CSS和架构进行修改和定制
- [x] 初步实现文档编写记录功能

- [x] 增加收藏页面

----

## 安装方式

1. 克隆本项目到本地
2. 安装插件

```bash
bundle install
```

3. 编译

```bash
jekyll build
```

4. 预览

如果你使用WSL 的话Jekyll 4.0 会因为实时预览而发生崩溃，无法通过CTRL+C退出预览，建议添加--no-watch

```bash
jekyll serve --no-watch
```

如果你在windows上或者linux平台下进行，可省略
