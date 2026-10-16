# 2026-009-ABB机器人实践

> ABB RobotStudio 实习实践项目，面向 IRB 2600-12/1.65 工站仿真、吸盘抓取与 RAPID 路径编程

## 项目效果图
![效果图](./b-Picture/效果图.png)

## 项目内容

1. **ABB实训工站一**
`a1-ABBPracticalTraining/` 为 RobotStudio 工站 ABBPracticalTraining。机型 IRB 2600-12/1.65 Type C，RobotWare 6.12.1014（中文、DeviceNet Master/Slave）。工站含吸盘工具 Tool_suck、工作台 table_and_fixture_140、工件「部件_1」，以及 SmartComponent_1（Attacher、Detacher、LogicGate、LineSensor），将控制器输出 do0 接到 di0。RAPID 主程序 `MainModule.mod` 使用 MoveAbsJ、MoveJ 与 Set/Reset do0 完成抓放路径。目录含 Station、Controller Data 与 Virtual Controllers。

2. **ABB实训工站二**
`a2-ABBPracticalTraining_1/` 为 RobotStudio 工站 ABBPracticalTraining_1。同为 IRB 2600-12/1.65，RobotWare 英文选项。含工具库 `Tool_suck.rslib`、末端工具 MyTool（SpintecTool）与工作台 table_and_fixture_140。RAPID 模块 `Module1.mod`（作者 cyx）使用 MoveAbsJ、MoveJ、MoveL、MoveC 编写直线与圆弧路径。目录含 Station 与 Controller Data。

3. **代码工站**
`b-Code/` 为 RobotStudio 工程 9-Code，含工站 `Station/9-Code.rsstnx`。当前工站为默认空站，仅有 RAPID 任务框架，未配置机器人本体与控制器数据。

4. **项目图片**
`b-Picture/` 存放 `效果图.png` 与 `Logo.png`。

5. **演示视频**
`b-Video/` 存放现场演示 `现场演示效果.mp4`，以及 `ABBPracticalTraining.exe`、`ABBPracticalTraining-2.exe`。

## 保留内容

### 学习许可与权利保留

- 本项目允许个人、学校和研究者进行非商业性的学习、研究和引用。
- 未经著作权人书面许可，不得将项目内容用于商业开发、产品制造、商业服务、商业宣传、投标交付、毕业设计成品交付或再授权。
- 不得删除作者、来源、版本历史和第三方许可证声明，不得将本项目或其衍生成果宣称为与作者无关的原创项目。
- 软件源码适用 [PolyForm Noncommercial 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0/)；机械模型、PCB、原理图、图片、文档、Unity 工程和其他非软件资料适用 [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)。
- SE、SW、STEP/STP 及其他三维模型仅允许个人或学校进行非商业学习、评审和研究；未经著作权人书面许可，不得用于加工、打样、制造、销售、量产、投标、产品交付、商业宣传、改作或再授权。
- 第三方组件、模板、元件库、外购件模型和工具仍受其原始许可证约束；本声明不扩大作者对第三方内容的权利。

商业使用、产品化、公司内部长期使用、转让或排他性授权需另行取得著作权人的书面许可。