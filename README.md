# 标准 Readme

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

标准 Readme 样式

README 文件是人们通常最先看到的第一个东西。它应该告诉人们为什么要使用、如何安装、以及如何使用你的代码。README 文件标准化能够使得创建和维护 README 文件更加简单。毕竟，要写好一个文档不是那么容易的。

本仓库包含以下内容：

1. 一个标准的 README 文件应该是什么样子的[规范](spec.md)。
2. 一个用于维护 README 文件的语法提示工具的链接 ([正在进行中](https://github.com/RichardLitt/standard-readme/issues/5))。
3. 一个创建标准 README 的[生成器](https://github.com/RichardLitt/generator-standard-readme)。
4. 一个指向该规范的[徽章](#徽章)。
5. [标准 README 的实例](example-readmes/) - 比如你正在读的这个文件。
标准 Readme 是为了开源组件设计的。尽管它的[背景](#背景)是为了服务于 Node 和 npm 项目, 它同时也可以应用到其他编程语言和包管理器中去。

## 内容列表

- [背景](#背景)
- [安装](#安装)
- [使用说明](#使用说明)
	- [生成器](#生成器)
- [徽章](#徽章)
- [示例](#示例)
- [相关仓库](#相关仓库)
- [维护者](#维护者)
- [如何贡献](#如何贡献)
- [使用许可](#使用许可)

## 背景

`标准 Readme` 最开始因为 [@maxogden](https://github.com/maxogden) 在项目 [feross/standard](https://github.com/feross/standard) 的[这个 Issue](https://github.com/feross/standard/issues/141) 中提出，是否标准化 README 会有助于帮助大家。很多人在仓库 [zcei's standard-readme](https://github.com/zcei/standard-readme/issues/1) 就这个想法进行了讨论。在我维护仓库 [IPFS](https://github.com/ipfs) 的时候，我需要在这个组织中推广标准化的 Readme，因此这个项目也就从这开始了。

> 如果你的文档是完整的，那么使用你代码的人就不用再去看代码了。这非常的重要。它使得你可以分离接口文档与具体实现。它意味着你可修改实现的代码而保持接口与文档不变。

> 请记住：是文档而非代码，定义了一个模块的功能。

—— [Ken Williams, Perl Hackers](http://mathforum.org/ken/perl_modules.html#document)

写 README 从某种程度上来说相当不易，一直维护下去更是难能可贵。如果可以减少这个过程，则可以让写代码与修改代码更容易，使得是否在说明中指明一处需改有无必要更加清楚，你可以花费更少的时间来考虑是否你最初的文档是否需要更新，你可以分配更多的时间来写代码而非维护文档。

同时，标准化在某些别的地方也有好处。有了标准化，用户就可以花费更少的时间来搜索他们需要的信息，他们同时可以做一个工具来从描述中搜集信息，自动跑示例代码，检查授权协议等等。

这个仓库的目标是：

1. 一个定义良好的**规范**。在仓库中的位置是 [spec.md](spec.md)。它是一个一直在持续优化的文档，欢迎您提 Issue 讨论其中的变化。
2. 一个**示例 README**。这个 Readme 完全遵从 Standard-readme，而且在 `example-readmes` 文件夹里有更多的示例。
3. 一个**语法提示器**用来提示在 Readme 中的语法错误。请参考 [tracking issue](https://github.com/RichardLitt/standard-readme/issues/5)。
4. 一个**生成器**用来快速搭建新的 README 的框架。请参考 [generator-standard-readme](https://github.com/RichardLitt/generator-standard-readme)。
5. 一个**标识准守规范的徽章**。请参考[徽章](#徽章)。

## 安装

编译安装环境
```sh
$ uname -a
Linux wtdcserver 5.4.0-73-generic #82~18.04.1-Ubuntu SMP Fri Apr 16 15:10:02 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux

$ java -version

java version "13.0.1" 2019-10-15
Java(TM) SE Runtime Environment (build 13.0.1+9)
Java HotSpot(TM) 64-Bit Server VM (build 13.0.1+9, mixed mode, sharing)

$ gradle -version
------------------------------------------------------------
Gradle 7.0.2
------------------------------------------------------------

Build time:   2021-05-14 12:02:31 UTC
Revision:     1ef1b260d39daacbf9357f9d8594a8a743e2152e

Kotlin:       1.4.31
Groovy:       3.0.7
Ant:          Apache Ant(TM) version 1.10.9 compiled on September 27 2020
JVM:          13.0.1 (Oracle Corporation 13.0.1+9)
OS:           Linux 5.4.0-73-generic amd64
```
![enviroment](readme_files/enviroment.png)

2. 克隆项目并进入项目

```sh
$ git clone https://gitee.com/dc-melo/standard-readme.git
OR
$ git clone https://github.com/DC-Melo/standard-readme.git
$ cd standard-readme
```

这个项目使用 [node](http://nodejs.org) 和 [npm](https://npmjs.com)。请确保你本地安装了它们。

```sh
$ npm install --global standard-readme-spec
```

## 使用说明

这只是一个文档包，你可以打印出 [spec.md](spec.md) 到输出窗口。

```sh
$ standard-readme-spec
# Prints out the standard-readme spec
```

### 生成器

想要使用生成器的话，请看 [generator-standard-readme](https://github.com/RichardLitt/generator-standard-readme)。
有一个全局的可执行文件来运行包里的生成器，生成器的别名叫 `standard-readme`。

## 徽章
如果你的项目遵循 Standard-Readme 而且项目位于 Github 上，非常希望你能把这个徽章加入你的项目。它可以更多的人访问到这个项目，而且采纳 Stand-README。 加入徽章**并非强制的**。 

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

为了加入徽章到 Markdown 文本里面，可以使用以下代码：

```
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
```

## 示例

想了解我们建议的规范是如何被应用的，请参考 [example-readmes](example-readmes/)。

## 相关仓库

- [Art of Readme](https://github.com/noffle/art-of-readme) — 💌 写高质量 README 的艺术。
- [open-source-template](https://github.com/davidbgk/open-source-template/) — 一个鼓励参与开源的 README 模板。

## 维护者

[@DC-Melo王江](https://github.com/DC-Melo)
[@DC-Melo王江](https://gitee.com/DC-Melo)

## 如何贡献

非常欢迎你的加入！[提一个 Issue](https://github.com/RichardLitt/standard-readme/issues/new) 或者提交一个 Pull Request。


标准 Readme 遵循 [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) 行为规范。

### 贡献者

感谢以下参与项目的人：
<a href="graphs/contributors"><img src="https://opencollective.com/standard-readme/contributors.svg?width=890&button=false" /></a>


## 使用许可

[MIT](LICENSE) © DC-Melo王江

## 捐赠 Donation

如果你喜欢我的项目，请在对应的项目右上角 "Star" 一下。你的支持是我最大的鼓励！ ^^ 你也还可以扫描下面的二维码，对作者进行打赏。

If you like my project, "Star" in the corresponding project right corner, please. Your support is my biggest encouragement! ^^ You can also scan the qr code below or Donate to this project using Paypal, donation to Author.
---
<div align="center">
<img src="readme_files/dc_wechat_pay.png" width="200" >
<img src="readme_files/dc_ali_pay.png"    width="200" >
<img src="readme_files/dc_bitcoin.png"    width="200" >
</div>

如果在捐赠留言中备注名称，将会被记录到列表中~ 如果你也是github开源作者，捐赠时可以留下github项目地址或者个人主页地址，链接将会被添加到列表中起到互相推广的作用

If you comment on the name in the donation message, it will be recorded in the list. ~If you are also an open source author of github, you can leave the GitHub project address or personal home page address when donating. Links will be added to the list to promote each other.
捐赠列表(Donation list)
# Project Name
Description

#### Background

#### Enviroment
```
$ uname -a
$ java -version
$ gradle -version
```

#### Build and Install

#### Usage

#### Badge

#### Maintainers

#### Related Efforts

#### Related Project

#### License









王江 DC-Melo
期待地点：海外北上杭深
岗位：图像算法,计算机3D建模渲染显示,计算机视觉图像理解
个人简介/开源项目：https://github.com/DC-Melo/README
联系方式：+86-152-1670-6941 wangjiang@alumni.tongji.edu.cn

工作经历&教育背景&主修课程
2019.5~至今     | 北京梧桐车联（腾讯与长安合资公司）         | 测试开发主管         | 汇报对象:测试总监
主要工作：HIL台架搭建，组织测试开发，构建测试原子方法，搭建测试框架,将中文用例转化为python代码填充到测试框架中，简单检查调试即可投入测试生产，测试工具集开发
20016.10~2019.4 | 安吉四维（安吉物流与四维图新合资公司）     | 技术部门主管         | 汇报对象:技术总监
主要工作：搭建导航系统测试系统，测试四维图新的导航地图。
2012.06~2016.09 | 上海翼锐汽车科技有限公司(上汽大众设计公司) | 仪表驾驶辅助测试主管 | 汇报对象:股长
主要工作：负责搭建大众MQB平台仪表测试系统和HUD测试系统、开发测试用例。
2009.09~2012.05 | 同济大学(985/211)                          | 汽车学院             | 硕士
主修课程：汽车试验、汽车动力学、现代控制理论、系统辨识、模糊控制、计算机控制基础、数学基础优异
2005.09~2009.06 | 江苏大学                                   | 汽车与交通工程学院   | 学士
主修课程：汽车构造、汽车理论、汽车电器、电路电子、自动控制理论、微机原理、汽车维修、汽车营销、管理学、数学基础优异

主要技能:
编程基础：| 编程工具                    | 对应工具链                      | 面向解决问题编程                        |
面向问题  | --------                    | ---                             | ---                                     |
快速学习  | 嵌入式,ASM,C/C++,uCos,Linux | CMake, GDB                      | HIL,OpenCV,OpenGL,FFmepg,SLAM,Blender3D |
编程技能  | JAVA                        | Gradle,JVM,SPring,Hadoop,Spark | APP开发，中间件开发,集群运算            |
          | Python                      | pudb                            | 数据爬虫，测试框架，tensorflow机器学习  |
          | Go                          |                                 | 跨平台系统命令                          |
兴趣涉猎：机器学习算法NB，DT，SVM，KF，TensorFlow、CNN、GAN，RNN，SLAM
数学基础：熟悉矩阵计算，熟悉概率论，熟悉复变函数，熟悉利群李代数
论文能力：读了较多的英文论文以及书籍。JVM，Introduction to Algorithms，Deep Learning（Lan Goodfellow），Deep Learning with Python，hadoop，spark

性格爱好																							
1. 无挑战不欢，性格开朗、富有挑战精神、喜欢尝试新鲜事物、喜欢有流动性的生活、有较强的适应性
2. 要玩就要玩专业，高级。喜欢运动。包括：摩托车、轮滑、滑雪、羽毛球，背包旅行
3. 喜欢展示分享，看各种论文，听分享报告

项目经验																							  
2019.05~至今			梧桐车联（腾讯CSIG智慧出行事业部）
Python：组织团队构建测试框架，开发python测试框架基础原子方法，将模版化的中文测试用例，通过vim编辑器快速生成测试用例脚本。团队经过简单调试，合校即可将上千条测试用例投入使用。
GO:     测试中心大约27个测试工具，按模块抓日志，获取各个APP版本号，运行monkey，检查ANR，CRASH，分析缺陷，自动提交缺陷等等。通过调研分析，GO语言非常适合做跨平台的命令工具。于是3天快速入门GO，两周完成27个功能中的20个功能的开发调试和使用培训。
JAVA:   使用JAVA开发了一安卓打地鼠游戏，用于采集车机不同屏幕区域的点击便捷度。
培训：  每月定期培训团队，赋能团队。培训内容包括: 嵌入式硬件基本知识，通讯基本知识基础,面向各种问题，使用对应编程语言解决问题。

2016.10~2019.04		安吉四维导航系统、导航地图测试、车辆互联产品开发测试
带领测试团队，组织安排车机测试工作。
测试基于Android的导航系统(给上汽红岩定制的产品)。具备Android系统定制能力(Linux+C编译)
测试手机车机互联产品(为大众、上汽定制的产品)。具备APP测试开发能力、adb调试能力(Linux+Java+adb)
基于ROS设计物流AGV仿真系统。使用blender画3D模型，使用gazebo进行仿真，使用OpenCV进行图像处理。

2012.09~2016.10		翼锐汽车仪表自动测试系统搭建
基于Python开发控制器一键快速编码程序(python)
基于CANoe开发控制器测试系统,进行CAN总线信号测试和硬线信号测试(C+CAN)
基于VB开发基于Excel测试用例管理系统、以及用户测试界面(VB)

2009.09~2011.04		研究生阶段参与课题：燃料电池备用电源控制器开发（国家科技支撑项目）
负责开发燃料电池备用电源人机界面，参与燃料电池备用电源系统控制流程设计 (Labview+C)
用Matlab验证模糊神经网络算法控制散热系统。并在Freescale(NXP)芯片的控制器上实现控制算法(NNs+C)。
移植实时操作系统uCos-II，并在uCos-II上实现系统的控制策略(汇编ASM+C语言)

开源项目,以及基于自己的一些想法的实现：
基于Opencv-python进行人脸识别，测试CNN识别算法(TensorFlow+CNN+Python+OpenCV)
利用FFmpeg和imagamagic制作自定义GIF动图(Linux+FFmpeg+imagmagic+Shell)
模拟wechat的web端API，批量发送定制化的祝福微信信息和定制化的GIF动图。利用该技术做汽车微信，通过汽车车机发送微信(AndroidStudio+Java)。
制作个人主页(LAMP)，制作公司考勤一览图(LAMP+Echarts)
制作公司bug跟踪系统(MantisBT)
制作个人位置跟踪记录APP(Java)，生成KML格式可以在google地图上回轨迹(AndroidStudio+Java)

奖励情况																							
2019.05~2019.12		三个专利		
2017.01~2017.02		获得年度优秀员工称号
2016.07~2016.07		“基于Excel的一键控制器编码”获得劳动竞赛最佳金点子
2014.08~2014.08		“基于数据库的半自动测试台架”获得大众联合创新大赛二等奖

Wang Jiang (王江)
+86-152-1670-6941 	2wangjiang@tongji.edu.cn
Vehicle Engineering in Tongji University, 4800# Cao’an Road, Shanghai, China 201804
Education                                                                      
Tongji University(985/211), Shanghai. 				                                            2009/09~now
M.S. expected in March 2011. Major in Vehicle Engineering;
Studied Modern control theory, system identification, fuzzy control, computer control base, automotive dynamics, auto test etc.
Jiangsu university, Jiangsu. 	                                                              2005/09~2009/06
B.S. in Automobile Application Engineering;
Studied Automobile structure, automobile theory, automobile electric appliances, circuit electronics, automatic control theory, car maintenance etc.
Internship Experience & Social Activity                                                       
Kunshan  Forsight Co. ,Ltd	 			         					                          2009, Kunshan
Backup power system field test; Researched uCos-II real-time operating system; developing the fuel cell backup power human-computer interface; design backup power system control process ;
Researched the current fuel cell development status and advanced technology;
Shanghai Fuel Cell Vehicle Powertrain Co., Ltd                       Jul. 2010~Aug. 2010, shanghai
Translated the oversea academic documents, and checked the translated documents;
Park technology Volunteer of Shanghai World Expo         			                    May.2010 shanghai 
Collected data of fuel cell car for Shanghai Automotive Industry Corporation (Group)
Project Experience													                                    
Participating project: Fuel cell backup power (national science and technology support project)                                                          Sep.2009~Now
analysis DC/DC outside characteristics,developed fuel cell backup power man-machine interface, participate in fuel cell backup power system control process design.
developed fuel cell backup power control system based on real-time operating system uCos – II.
Researching project: fuel cell generator                        			               Sep.2009~Mar.2011
developed monomer inspection program;
Researching topic: fuel cell system control                        			               Sep.2009~Now
research fuel cell system output capacity, and the relationship between fuel cell system working efficiency and system  working point.
research real-time operating system uCos - II.
research neural network and fuzzy control theory.
Skills																			                            
Programming Software: C Language, Matlab(simulink), Test Software(Labview)
Designing Software: AutoCAD, Hypermes
English：CET-6
Editing Software: Word, Excel, PowerPoint 
