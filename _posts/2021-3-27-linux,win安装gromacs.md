---
layout:     post
title:      gromacs安装
subtitle:   Linux，win
date:       2021-03-27
author:     xiaodechao
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - manjaro
    - gromacs安装
    - 分子动力学模拟
    - 入门
---
# 1  gromacs简单安装#
## (1)ubuntu/centos系统安装##
使用命令安装

    sudo apt-get install gromacs

## (2)manjaro 安装gromacs ##
打开应用商店（打开首选项，启用其它的软件库），搜索gromacs，下载gromacs

或者命令安装

    yaourt gromacs 

    yay gromacs


注意： 

yaourt和yay命令需要通过sudo pacman -S name 安装获得


## (3)win10安装gromacs ##
1 在win10系统的控制面板点击程序和动能的‘启用或关闭window功能’

2 点击‘适用Linux的windows子系统’，然后点击‘确定’。

3 然后，重启电脑。重启电脑后，在Microsoft Store搜索ubuntu下载即可，下载好，点击‘启用’。

4 按照提示，随便起个username，输入密码，切记密码记住。ps：输入过程中密码不会显示，输入后点击enter就行。会让输入两次确定密码是否一致。之后再用的话可以在任务中找到，ubuntu，点击即可。

5 为避免安装缺少东西，第一步，输入sudo apt update，enter之后等待完成。第二步，输入sudo apt upgrade，enter之后等待完成。第三步，输入sudo apt-get gromacs，就会自动安装gromacs，时间大约10多分钟。

## (4)详细安装 ##

> http://sobereva.com/457
