# Blender 5.2.0 DLSS Preview – Pre-release Notes

本版本为预发行版，尚不稳定，不建议用于正式生产环境。如遇问题请提交反馈。

---

## English

### Overview
This is an unofficial preview build of Blender 5.2.0 with experimental DLSS Ray Reconstruction support for Cycles.

DLSS will be officially integrated into Blender 5.3. This build is intended for early testing only.

### Requirements
- GPU: NVIDIA RTX series only (Tensor Core required)
- Driver: NVIDIA Display Driver version 590 or higher
- GTX series GPUs do not have Tensor Cores and cannot enable DLSS.

### Important Notes
- This is an experimental custom build, not an official Blender Foundation release. Instability, crashes, or visual artifacts may occur.
- DLSS is proprietary NVIDIA NGX technology.
- Recommended for interactive viewport preview only. For final rendering, please complete thorough verification before output.
- Built from the official Blender main branch source code. Only build configuration parameters were modified to enable DLSS, CUDA, and OptiX. No source logic was altered.
- For build reproduction commands, please refer to the documents in this repository.

### License
- Blender source code is governed by GNU GPLv3.
- This build links against the closed-source NVIDIA DLSS SDK, which is subject to the NVIDIA EULA.
- This preview build is for non-commercial testing only.

---

## 中文

### 概览
本版本是非官方编译预览版 Blender 5.2.0，为 Cycles 渲染器开启实验性 DLSS 光线重建功能。

DLSS 将在 Blender 5.3 官方正式上线，本构建用于提前测试。

### 使用要求
- 显卡：仅限 NVIDIA RTX 系列（需要 Tensor Core）
- 驱动：NVIDIA 显卡驱动版本 590 或更高
- GTX 系列显卡无 Tensor Core，无法启用 DLSS 功能。

### 重要注意事项
- 属于实验性定制构建，并非 Blender 基金会官方版本，可能存在不稳定、闪退、画面异常等问题。
- DLSS 为 NVIDIA 私有 NGX 技术。
- 建议仅用于视口交互预览；最终成品渲染前请充分测试验证。
- 基于 Blender 官方主线源码编译，仅修改编译配置参数，开启 DLSS、CUDA、OptiX 选项，未修改源代码逻辑。
- 复现编译所需命令可查阅仓库内文档。

### 许可证说明
- Blender 原始源码遵循 GNU GPLv3 开源协议。
- 本构建链接闭源 NVIDIA DLSS SDK，受 NVIDIA 终端用户协议约束。
- 本预览构建仅供非商业测试使用。

---
