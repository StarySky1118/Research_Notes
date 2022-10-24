# 教程使用方法

SOAR 官网链接：https://soar.eecs.umich.edu/articles/articles。

SOAR 9.6.0 Tutorial 链接：https://soar.eecs.umich.edu/articles/downloads/soar-suite/228-soar-tutorial-9-6-0。

**教程功能**

1、介绍 Soar 基本运行原理

2、运行 Soar 程序、理解 Soar 程序的运行

3、如何写出自己的 Soar 程序

**使用步骤：**

1、下载 Soar 9.6.0 Tutorial Multi-Platform，解压。

> 路径名中不能有空格和圆括号。

2、读每一章教程。

3、运行教程中的 Soar 程序

windows：运行 `SoarJavaDebugger.bat`。

> 条件：64 位操作系统；安装 jre。

**延伸阅读：**

Soar Mannal

Gentle Introduction to Soar

# Tutorial.1 Simple Agents

## Introduction

Soar 是建立智能系统的统一架构，提供一个固定的计算结构，在这个结构中，知识可以被编码并用来产生追求目标的行为。Soar 在很多方面像一门编程语言，尽管是一门专用的语言。Soar 区别于其他编程语言的点在于，它嵌入了一种特定的理论，这种理论由合适的基本体组成，这些基本体隐含推理、学习、计划和其他一些对于智能行为很有必要的能力。Soar 的目标不是建立一个通用编程语言，某些数学计算过程在 Soar 中很困难或很别扭，这些计算过程更适合在 C, C++ 和 Java 中实现。Soar 适合建立**使用大量知识产生行为、追求目标的、自主的**智能体。

Soar 有独立的编辑器：VisaulSoar。

## Part I: Simple Soar Programs

### 1、安装 Soar

在 教程使用方法 --》 使用步骤 中。

### 2、使用规则建立简单的 Soar Agent

Soar Agent 中所有知识使用 if-then 规则表示。在 Soar 中，规则被称为 production。规则被用来选择和应用到 operator 上。

#### 2.1 创建 Soar Agent 和使用 Soar Debugger 

打开 `SoarJavaDebugger.bat` 启动 Soar，打开的窗口就是 Soar Debugger，如下图所示：

![image-20221024154627236](img/SoarDebugger.png) 

> 左侧空白区域：交互窗口，显示调试信息和打印语句。

> 空白区域下方：命令盒，输入命令。

打开 Soar Debugger 后，将自动创建名为 soar1 的默认 agent，其名称显示在窗口标题。

运行 Soar 程序时，可以通过点击按钮或输入命令执行操作，如下所示：

![image-20221024160925821](img/Command.png)

#### 2.1 Hello-World 规则

