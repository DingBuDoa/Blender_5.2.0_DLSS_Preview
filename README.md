# Blender_5.2.0_DLSS_Preview

## English
This is an unofficial manually compiled preview build of Blender 5.2.0, which adds experimental DLSS Ray Reconstruction support for the Cycles path tracer.

### Introduction
NVIDIA DLSS (Deep Learning Super Sampling) is widely recognized as an AI acceleration technology.
Most users first encounter DLSS in 3A real-time games to boost frame rates with ray tracing enabled.
Nowadays, it is also commonly used in real-time virtual production and architectural visualization to optimize viewport performance.

So what if we apply DLSS AI acceleration to offline industrial 3D rendering?

Official Blender 5.2 does not integrate DLSS modules. Native DLSS Ray Reconstruction support for Cycles will come with Blender 5.3.
This custom build enables artists to test the feature in advance for product rendering, mechanical design visualization and architectural scenes.

DLSS Ray Reconstruction serves as an advanced AI denoiser and detail reconstructor.
It removes heavy viewport noise under low sampling values while preserving clear reflections, refractions and subtle lighting details.
It drastically cuts waiting time during iterative material, lighting and lookdev adjustments.

### Mandatory Hardware & Driver Requirements
1. Graphics Card: **NVIDIA RTX GPU only**. GTX GPUs do not have Tensor Cores and cannot activate DLSS.
2. Display Driver: Minimum NVIDIA driver version **590**. Older drivers may trigger crashes or disable DLSS functions.

### Important Disclaimer
- This is an experimental custom build, **not official software released by the Blender Foundation**. Potential instability may exist.
- DLSS is proprietary NVIDIA NGX technology. Feature availability relies on your graphics driver runtime.
- Recommended for interactive viewport preview. Conduct sufficient verification before final output rendering.
- Official stable DLSS support will be available in Blender 5.3.

### Build Information
Compiled from Blender main branch source code on Windows.
CUDA, OptiX and DLSS SDK are enabled during compilation.

### License
Blender original source code is licensed under the **GNU General Public License v3.0 (GPLv3)**.
This custom build links against NVIDIA DLSS SDK, a proprietary library governed by NVIDIA End User License Agreement (EULA).
The DLSS component is closed-source and incompatible with GPLv3 terms.
This preview build is provided for non-commercial testing purposes only.

Base upstream source: https://projects.blender.org/blender/blender
This build is compiled from official Blender main branch source, only build configuration parameters are adjusted to enable DLSS, OptiX and CUDA.
No manual modification to the source code logic. You can reproduce this build using the build command provided in this repository.

---

## 中文
本项目是非官方手动编译的 Blender 5.2.0 预览构建版，为Cycles路径追踪渲染器增加实验性DLSS光线重建功能。

### 简介
NVIDIA DLSS（深度学习超级采样）是知名的AI加速技术。
大部分人最先在3A实时游戏中接触到它，开启光追的同时有效提升画面帧率。
如今这项技术也大量应用于实时虚拟制片、建筑可视化项目，优化视口交互流畅度。

如果将DLSS AI加速技术运用到离线工业3D渲染中，会带来怎样的变化？

正式版 Blender 5.2 并未内置DLSS相关模块，Cycles的DLSS光线重建功能将在Blender 5.3官方上线。
这份定制编译版本，可以让产品渲染、机械可视化、建筑效果图创作者提前体验该特性。

DLSS光线重建相当于一套高阶AI降噪与细节重建方案。
在低采样设置下有效消除视口噪点，同时保留清晰反射、折射与细微光影信息，大幅缩减材质、灯光反复调试的等待时间。

### 硬性硬件与驱动要求
1. 显卡：**仅支持NVIDIA RTX系列显卡**。GTX显卡缺少Tensor Core，无法启用DLSS。
2. 显卡驱动：最低驱动版本 **590**，低于该版本可能出现渲染闪退、DLSS功能失效。

### 重要声明
- 这是实验性自定义编译版本，**不属于Blender基金会官方程序**，存在不稳定风险。
- DLSS属于NVIDIA私有NGX技术，功能可用性取决于显卡驱动运行环境。
- 适合视口交互预览使用，最终成品渲染前请充分测试验证。
- 稳定的官方DLSS支持将在Blender 5.3版本到来。

### 编译信息
基于Windows环境编译Blender主线源码，编译时开启CUDA、OptiX、DLSS SDK

### 许可证说明
Blender 原始源码遵循 **GNU General Public License v3.0 (GPLv3)** 开源协议。
本定制构建链接了 NVIDIA DLSS SDK，该组件为专有闭源软件，受NVIDIA终端用户许可协议(EULA)约束。
DLSS相关库不属于开源代码，与GPLv3存在协议不兼容问题。
本预览编译版本仅供非商业测试使用。

上游源码地址：https://projects.blender.org/blender/blender
本构建基于官方Blender主线源码编译，仅调整构建配置参数，启用DLSS、OptiX、CUDA编译选项，未手动修改源代码逻辑。你可以使用仓库内提供的编译命令复现相同版本。
