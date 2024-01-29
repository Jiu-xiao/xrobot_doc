---
title: xPSR
layout: default
parent: Cortex-M3
grand_parent: Learn
nav_order: 10
---

# xPSR

---
xPSR (Program Status Register 程序状态寄存器)，x代表xPSR由三个小寄存器组成。分别包括：

* APSR （Application Program Status Register 应用程序状态寄存器)
* IPSR （Interrupt Program Status Register 中断程序状态寄存器）
* EPSR (Execution Program Status Register 执行程序状态寄存器)
![](/img/images/screenshot_1653109583440.png)
蓝色部分是 APSR，占领了高 27bit ~ 31bit，紫色部分是 EPSR，占领了高 9bit ~ 26bit，绿色部分是 IPSR，占领了低 0bit ~ 8bit
