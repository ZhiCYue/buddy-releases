<div align="center">
  <h1>Buddy</h1>
  <p>住在菜单栏里的 AI 智能体助手 —— 每个智能体是一只可点击对话的桌面小宠物。</p>
</div>

## 下载

前往 **[Releases](../../releases/latest)**，下载对应平台的安装包：

| 平台 | 文件 |
|------|------|
| macOS（Apple 芯片 / M 系列） | `Buddy-<版本>-arm64.dmg` |
| Windows | `Buddy-<版本>-x64.exe` |
| Linux | `Buddy-<版本>-x86_64.AppImage` |

## 安装

### macOS

1. 打开下载的 `.dmg`，把 **Buddy** 拖进「应用程序」，然后推出磁盘映像。
2. Buddy 没有 Dock 图标 —— 启动后在**屏幕顶部菜单栏**找它的小图标。

首次打开若提示 **「Buddy 已损坏，无法打开」**，打开「终端」执行下面两条，然后重新打开：

```bash
xattr -cr /Applications/Buddy.app
codesign --force --deep --sign - /Applications/Buddy.app
```

> Intel 芯片通常只需第一条；Apple 芯片两条都执行。

### Windows

双击 `Buddy-<版本>-x64.exe` 安装。若 SmartScreen 拦截，点「更多信息 → 仍要运行」。安装后 Buddy
在**系统托盘**（任务栏右下角）。

### Linux

给 AppImage 加可执行权限后运行：

```bash
chmod +x Buddy-<版本>-x86_64.AppImage
./Buddy-<版本>-x86_64.AppImage
```

> 部分桌面环境（如 GNOME）需安装 AppIndicator/StatusNotifier 扩展，托盘图标才会显示。

## 使用

- 点菜单栏 / 托盘图标：新建、编辑、显示/隐藏你的智能体。
- 桌面上的小宠物：点一下即可和它对应的智能体对话；右键可关闭。
- 在设置里填入你的模型 API Key 即可开始使用。

---

有问题欢迎在 [Issues](../../issues) 反馈。
