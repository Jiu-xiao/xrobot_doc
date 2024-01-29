---
title: BASEPRI
layout: default
parent: Cortex-M3
grand_parent: Learn
nav_order: 6
---

# BASEPRI
---
这个寄存器最多有 9 bit（由表达优先级的位数决定）。它定义了被屏蔽优先级的阈值；换言之，当这个寄存器被设置某个数值后，所有优先级号大于等于该值的中断都被关闭（优先级号越大，优先级越低）；默认值是0，也就是不关闭任何中断；