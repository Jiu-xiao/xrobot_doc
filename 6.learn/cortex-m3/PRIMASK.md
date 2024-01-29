---
title: PRIMASK
layout: default
parent: Cortex-M3
grand_parent: Learn
nav_order: 9
---

# PRIMASK
---
只有单一 bit 的寄存器。当它被置位 1 后，就关掉了所有可屏蔽的异常（中断），只剩下 NMI 和 HardFault 可以响应。
注意，PRIMASK只是屏蔽掉中断，而并不是不让中断源产生中断