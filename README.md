# Kaenx.Creator
Kaenx.Creator汉化版
# Kaenx.Creator（Kaenx-Creator）

**OpenKNX 项目下的 Windows 桌面工具，C# 开发，用于生成 KNX 设备描述文件 `knxprod`，给 ETS 软件使用**

> 
> 正好和你前面 HomeAssistant 自定义集成的设备日志相关：`knxprod` 就是 KNX 设备的产品定义、对象、通道映射文件。

## 核心用途

1. 可视化编辑 KNX 设备：产品信息、通信对象（GroupObject）、参数、内存布局、应用程序
2. 导出 **`.knxprod`**，ETS5.6+ 可以直接导入，作为自定义 KNX 设备库
3. 支持 OpenKNX、Selfbus 自制 KNX 硬件（ESP32/STM32 KNX 节点）
4. 附带命令行版本 `Kaenx-Creator-Console`，支持脚本批量生成

## 仓库

GitHub：[https://github.com/OpenKNX/Kaenx-Creator](https://github.com/OpenKNX/Kaenx-Creator)

- 主程序：`Kaenx.Creator`（GUI）
- 源码 .NET 框架，Windows 运行
- 模型定义素材仓库：Kaenx-Creator-Share

## 简单工作流

1. 新建项目 → 填写设备产品 ID（类似你日志里 `product 007`）
2. 添加通信对象、参数块
3. 配置应用程序、硬件内存
4. 导出 `.knxprod`
5. 在 ETS 导入 knxprod，即可添加这个自制 KNX 设备到项目
<img width="2576" height="1420" alt="图片" src="https://github.com/user-attachments/assets/f4710581-068e-422a-acc2-76048f2c2eaa" />
<img width="2565" height="1417" alt="图片" src="https://github.com/user-attachments/assets/c3a660df-cb8d-4cf6-938e-a14e7eac398b" />
