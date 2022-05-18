# MurphySec Code Scan

<a href="https://www.jetbrains.com"><img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg" width = "10%" /></a>

[![](https://badgen.net/badge/Github/murphysec-code-scan/21D789?icon=github)](https://github.com/murphysecurity/murphysec-jetbrains-plugin)
![Version](https://img.shields.io/jetbrains/plugin/v/18274?logo=JetBrains)
![Downloads](https://img.shields.io/jetbrains/plugin/d/18274?color=FE2857)
![Rating](https://img.shields.io/jetbrains/plugin/r/rating/18274?color=3EB811)

[**MurphySec Code Scan**](https://plugins.jetbrains.com/plugin/18274-murphysec-code-scan) 是[墨菲安全](https://www.murphysec.com/)推出的一款 JetBrains IDE 插件。


该插件让开发者在 IDE 中即可检测代码依赖的安全问题，轻松识别代码中使用了哪些存在安全缺陷的开源组件，通过准确的修复方案和一键修复功能，快速解决安全问题。

### 支持功能

目前 Murphysec Code Scan 支持的功能如下：
- 漏洞检测：检测 `Java(Maven)`、`JavaScript(npm)`、`Go(gomod)`、`Python(pip)` 代码中引入的缺陷组件
- 一键修复：不仅有清晰的修复方案，还可以通过此功能快速修复
- 实时检测：代码的依赖发生变化导致了安全问题，不用担心，插件会及时给您提醒进行处理


> 注意
> 此插件不支持2020.1之前版本的JetBrains IDE

## 安装插件
- 打开 IDE 并进入插件市场
- 在插件市场中搜索 “Murphysec Code Scan”，查看详情并安装

 
![plugin-install2](./screenshot/plugin-install2.png)


## 配置插件
1. 点击下方插件区域左侧的`设置`按钮，或点击引导中的`服务认证`
2. 在弹窗中输入您的访问令牌，也可以点击`快速认证`按钮按照引导完成认证。

![plugin-config1](./screenshot/plugin-config1.png)
![plugin-config2](./screenshot/plugin-config2.png)




**配置参数说明：**
1. token：进入[墨菲安全控制台](https://www.murphysec.com/control/set)，点击“个人设置”，如下图所示：

![api-token](./screenshot/api-token.png)
2. 企业配置 - 服务地址：如果想使用墨菲安全私有化部署的服务，请填写服务地址（如果没有，可以不填写）
## 如何使用

### 开始扫描
- 点击 IDE 下方菜单栏中的“MurphySec Code Scan”，选择`点击开始扫描`
 
![plugin-start](./screenshot/plugin-start.png)

### 查看扫描结果
- 扫描完成后会在窗口内显示结果，可以点击左侧漏洞查看详细信息

![plugin-result](./screenshot/plugin-result.png) 

### 修复

- 点击检测结果中的组件，即可查看该缺陷组件的基本信息
- 点击右侧“一键修复”，即可直接将该组件升级至“最小修复版本

点击下方的`一键修复`按钮，即可直接将该组件升级至最小修复版本

![plugin-quick-fix](./screenshot/plugin-quick-fix.png) 

### 重新扫描
- 点击插件左侧选项栏中的`绿色开始图标`，即可重新扫描

![plugin-restart](./screenshot/plugin-restart.png)


## 常见问题

### 1. 将插件从 sidebar 移除了，我要怎么检测？

- 点击菜单栏上的 `View` -> `Tool Windows` -> `MurphySec` ，插件将会重新出现在 sidebar 上
![plugin-sidebar](./screenshot/plugin-sidebar-murphysec.jpeg)