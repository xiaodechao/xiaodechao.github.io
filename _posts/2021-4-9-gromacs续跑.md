---
layout:     post
title:      gromacs续跑
subtitle:   gromacs中断，模拟时间延长
date:       2021-4-9
author:     xiaodechao
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - gromacs
    - 续跑
    - 延长模拟时间
---
# 1 gromacs模拟结束，继续跑 #

    gmx convert-tpr -s md.tpr -extend 2000 -o md1.tpr

    gmx mdrun -v -deffnm md1 -cpi md.cpt -noappend

-s md.tpr 输入生成md.tpr文件
-extend 2000 延长2000ps
-o md1.tpr 输出新的tpr文件

-deffnm md1 生成的文件名

# 2 gromac中断，续跑 #

中断的任务是这样运行的：

    gmx mdrun -deffnm md

在同一个文件夹下运行：

    gmx mdrun -s md.tpr -cpi md.cpt -deffnm md

