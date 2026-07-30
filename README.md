# PICO Unity Project Templates

## 中文

本仓库包含两个 PICO Unity SDK 工程模板，分别对应 PICO XR 和 Unity OpenXR 两种接入模式。每个子目录都是一个可直接用 Unity 打开的独立工程。

### 模板目录

| 目录 | 模式 | 说明 |
| --- | --- | --- |
| `PICOXR` | PICO XR | 基于 PICO XR 模式的工程模板，适合直接使用 PICO Unity SDK / PICO XR 能力进行开发。 |
| `OpenXR` | Unity OpenXR | 基于 Unity OpenXR 模式的工程模板，适合使用 Unity OpenXR 工作流并结合 PICO Unity SDK 能力进行开发。 |

### Unity 版本

两个模板当前使用的 Unity Editor 版本一致：

```text
6000.0.73f1
```

建议使用相同版本的 Unity 打开工程，以减少包解析、工程设置或导入结果差异。

### 使用方式

1. 安装 Unity `6000.0.73f1`，并确保已安装 Android Build Support。
2. 根据需要选择模板目录：
   - 使用 PICO XR 模式时，打开 `PICOXR`。
   - 使用 Unity OpenXR 模式时，打开 `OpenXR`。
3. 在 Unity Hub 中选择 `Add project from disk`，然后选择对应的模板目录。
4. 等待 Unity Package Manager 完成依赖解析和资源导入。
5. 在 Unity 中切换到 Android 平台后进行开发、调试和构建。

### 依赖说明

模板工程通过 `Packages/manifest.json` 引用 PICO Unity SDK 相关包，以及 Unity XR、Input System、URP 等常用依赖。首次打开工程时需要网络访问 GitHub 和 Unity Package Registry。

### 适用场景

- `PICOXR`：适合以 PICO XR SDK 为主要运行时接入方式的 PICO 设备项目。
- `OpenXR`：适合以 Unity OpenXR 为主要运行时接入方式，并需要保持 OpenXR 工作流一致性的项目。

### 目录结构

```text
.
├── OpenXR/
│   ├── Assets/
│   ├── Packages/
│   └── ProjectSettings/
└── PICOXR/
    ├── Assets/
    ├── Packages/
    └── ProjectSettings/
```

## English

This repository contains two PICO Unity SDK project templates for the PICO XR and Unity OpenXR integration modes. Each subdirectory is an independent Unity project that can be opened directly in Unity.

### Template Directories

| Directory | Mode | Description |
| --- | --- | --- |
| `PICOXR` | PICO XR | Project template based on the PICO XR mode. Use this when developing directly with PICO Unity SDK / PICO XR features. |
| `OpenXR` | Unity OpenXR | Project template based on the Unity OpenXR mode. Use this when following the Unity OpenXR workflow while integrating PICO Unity SDK features. |

### Unity Version

Both templates currently use the same Unity Editor version:

```text
6000.0.73f1
```

It is recommended to open the projects with the same Unity version to reduce differences in package resolution, project settings, and imported assets.

### Usage

1. Install Unity `6000.0.73f1` and make sure Android Build Support is installed.
2. Choose the template directory based on your integration mode:
   - Open `PICOXR` for the PICO XR mode.
   - Open `OpenXR` for the Unity OpenXR mode.
3. In Unity Hub, select `Add project from disk`, then choose the corresponding template directory.
4. Wait for Unity Package Manager to resolve dependencies and import assets.
5. Switch the project to the Android platform in Unity before development, debugging, and building.

### Dependencies

The template projects reference PICO Unity SDK packages and common Unity dependencies such as Unity XR, Input System, and URP through `Packages/manifest.json`. Network access to GitHub and Unity Package Registry is required when opening a project for the first time.

### Use Cases

- `PICOXR`: Suitable for PICO device projects that use PICO XR SDK as the primary runtime integration mode.
- `OpenXR`: Suitable for projects that use Unity OpenXR as the primary runtime integration mode and need to keep a consistent OpenXR workflow.

### Directory Structure

```text
.
├── OpenXR/
│   ├── Assets/
│   ├── Packages/
│   └── ProjectSettings/
└── PICOXR/
    ├── Assets/
    ├── Packages/
    └── ProjectSettings/
```
