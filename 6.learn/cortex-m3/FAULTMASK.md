---
title: FAULTMASK
layout: default
parent: Cortex-M3
grand_parent: Learn
nav_order: 7
---

# FAULTMASK
---
也是只有 1 bit 的寄存器，当设置为 1 的时候，只有 NMI 才能够响应，其他所有的异常，甚至是 HardFault 也不响应，默认值是 0，也就是都响应；