---
layout: post
title:  "Archlinux 安装记录"
date:   2020-03-01 18:11:13
categories: Linux
tags: ['ArchLinux','Linux']
excerpt: Archlinux 安装过程记录
---
* content
{:toc}

## Arch Linux 安装

### 制作Live CD

1. [下载镜像](https://www.archlinux.org/download/)

2. 制作USB 启动工具,采用dd方式写入

![](/assets/post-img/linux/refus.PNG){:.img-default}

3. 双系统下的准备工作

在windows 磁盘管理工具中空出一块未分配分区

![](/assets/post-img/linux/disk.PNG){:.img-fixed-50}

## 启动Live CD

重启后在引导中选择UEFI模式的Archlinux。

![](/assets/post-img/linux/arch-boot.PNG){:.img-default}

### 联网和源更新

1. 网络连接

```bash
wifi-menu
ping www.baidu.com 
```

2. 源更新

```bash
vim /etc/pacman.d/mirrorlist
# 网易
Server = http://mirrors.163.com/archlinux/$repo/os/$arch
# 清华大学 TUNA 协会
Server = https://mirrors.tuna.tsinghua.edu.cn/archlinux/$repo/os/$arch
# 中国科学技术大学
Server = https://mirrors.ustc.edu.cn/archlinux/$repo/os/$arch
# 西安交通大学
Server = https://mirrors.xjtu.edu.cn/archlinux/$repo/os/$arch
```

3 . 更新

```bash
pacman -Syy && pacman -S archlinuxcn-keyring && pacman -Syyu
pacman -S vim git 
```

## 分区

采用cfdisk对磁盘进行分区

![](/assets/images/linux/cfdisk.PNG){:.img-default}

```bash
lsblk
cfdisk
```

习惯不用Swap分区，不分home 分区，**只分/分区**

