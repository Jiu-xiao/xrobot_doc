---
title: Start
layout: default
parent: Advanced
nav_order: 1
has_children: true
---

# 开始

如何从头开始为一块开发板创建对应的BSP，编写板载设备的驱动，设计特定功能的模块，最后组合成你自己的机器人。

## 注意

新加入任何源文件和头文件之后，如果想要编译他们或者在文件中启用VSCode的自动补全，必须要在配置中选择此模块(`./project.py config`），然后重启VSCode或者刷新CMake缓存（`./project.py refresh`）。
