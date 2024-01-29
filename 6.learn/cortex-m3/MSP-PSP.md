---
title: MSP/PSP
layout: default
parent: Cortex-M3
grand_parent: Learn
nav_order: 8
---

# MSP/PSP

CM3 处理器使用的是 “向下生长的满栈” 模型。向下生长是指栈底在高地址，入栈时栈顶向低地址移动。满栈是指栈指针指向栈顶的第一个元素。
CM3支持双堆栈，即MSP(主堆栈指针) PSP（用户堆栈指针），他们的切换参考特殊功能寄存器CONTROL[1]。
裸机的情况下不对系统进行保护，用户代码跑在特权模式，默认使用MSP。handle/中断时也使用MSP作为堆栈指针。这种情况下的 PSP 与 MSP 切换，是硬件自动完成并压栈的。
![](/img/images/screenshot_1653116355430.png)
跑RTOS时，每个线程都有自己的堆栈，使用PSP将系统堆栈和用户堆栈分开。OS 可以手动压栈弹栈，修改 PSP 来达到切换任务上下文目的。
![](/img/images/screenshot_1653116394887.png)
