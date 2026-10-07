# 最后生还者 MOD 管理器 v1.1.46

这是《The Last of Us Part I》Steam 版的 MOD 管理器。

## 中文教程

### 一、安装和首次设置

1. 将发布压缩包解压到一个独立文件夹。
2. 运行 TLOU Mod Manager.exe。
3. 点击“选择目录”，选择游戏根目录。
4. 正确的游戏根目录中应同时存在：
   - tlou-i.exe
   - build\pc\main
5. 第一次使用时点击“扫描游戏归档”，等待扫描完成。
6. 在“MOD目录”中选择存放 MOD 的文件夹，然后点击“刷新列表”。

请先关闭游戏，再安装、切换或卸载 MOD。

### 二、添加和启用 MOD

1. 将 MOD 文件夹或 MOD 包放入管理器当前设置的 MOD 目录。
2. 点击“刷新列表”。
3. 在 MOD 列表中勾选需要使用的 MOD。
4. 点击“安装/应用”，或按照管理器界面提示完成安装。
5. 启动游戏并查看效果。

普通 MOD 文件夹必须包含 build\pc\main，例如：

    我的MOD
    ├─ build
    │  └─ pc
    │     └─ main
    │        └─ actor97
    │           └─ example.pak
    ├─ modinfo.ini       （可选）
    └─ preview.jpg       （可选）

### 三、卸载 MOD

1. 关闭游戏。
2. 在 MOD 列表中取消勾选要移除的 MOD。
3. 点击“刷新列表”或“安装/应用”。
4. 管理器会恢复被该 MOD 修改的文件。

如果同时使用多个 MOD，建议一次只启用一个新 MOD。出现冲突时，先取消最近启用的 MOD，再逐个测试。

### 四、支持的文件格式

- MOD 文件夹：文件夹中必须有 build\pc\main。
- .tlou1mod：由 V夭魔 制作的 MOD 格式。
- .zip 或 .rar：压缩包中必须有 build\pc\main。

### 五、填写 MOD 名称和预览图

可以在 MOD 根目录放置 modinfo.ini。可复制程序附带的 modinfo-template.ini 后修改。

    [ModInfo]
    Name=MOD 名称
    Author=作者
    Version=1.0
    Screenshot=preview.jpg
    ReplacesZh=替换内容
    DescriptionZh=MOD 说明

预览图支持 PNG、JPG、JPEG；缩略图也支持 BMP。Screenshot 必须填写 MOD 根目录中的实际图片文件名，例如 preview.jpg。不填写时，管理器会自动查找常见的 screenshot、preview、cover 或 thumbnail 图片。

### 七、常见问题

- 列表中没有 MOD：确认文件放在管理器当前设置的 MOD 目录，然后点击“刷新列表”。
- 提示游戏目录不正确：重新选择同时包含 tlou-i.exe 和 build\pc\main 的目录。
- 提示 MOD 结构不正确：确认文件夹或压缩包内存在 build\pc\main。
- 安装失败：关闭游戏，重新扫描游戏归档，再刷新 MOD 列表。
- 游戏出现异常：先卸载最近启用的 MOD，只保留一个 MOD 进行测试。
- 想恢复原状：取消勾选对应 MOD，然后重新应用设置。
- 管理器显示已有实例：关闭已经运行的管理器窗口后再启动。
- - - - - - - - - - - - - - - - - - - - - - - - -- 
# The Last of Us MOD Manager v1.1.46

This tool manages mods for the Steam version of The Last of Us Part I.

## English Guide

### 1. Installation and first-time setup

1. Extract the release archive to its own folder.
2. Run TLOU Mod Manager.exe.
3. Click Browse and choose the game root folder.
4. The selected game root must contain both:
   - tlou-i.exe
   - build\pc\main
5. On first use, click Scan game archives and wait for the scan to finish.
6. Choose the folder where you keep your mods in MOD folder, then click Refresh.

Close the game before installing, switching, or removing a mod.

### 2. Add and enable a mod

1. Put a mod folder or mod package in the MOD folder selected in the manager.
2. Click Refresh.
3. Check the mod in the mod list.
4. Click Install/Apply, or follow the action shown by the manager.
5. Start the game and test the result.

A normal mod folder must contain build\pc\main. Example:

    MyMod
    ├─ build
    │  └─ pc
    │     └─ main
    │        └─ actor97
    │           └─ example.pak
    ├─ modinfo.ini       (optional)
    └─ preview.jpg       (optional)

### 3. Remove a mod

1. Close the game.
2. Uncheck the mod you want to remove.
3. Click Refresh or Install/Apply.
4. The manager restores files changed by that mod.

When using several mods, enable one new mod at a time. If a conflict appears, disable the most recently enabled mod and test again.

### 4. Supported file formats

- Mod folders: the folder must contain build\pc\main.
- .tlou1mod: the MOD package format created by Vyaomo.
- .zip or .rar: the archive must contain build\pc\main.

### 5. Add mod information and a preview image

You can place modinfo.ini in the root of the mod folder. Copy the included modinfo-template.ini and edit it.

    [ModInfo]
    Name=Mod name
    Author=Author
    Version=1.0
    Screenshot=preview.jpg
    ReplacesEn=What this mod replaces
    DescriptionEn=Description of the mod

Preview images can be PNG, JPG, or JPEG; BMP is also supported for thumbnails. Screenshot must be the exact image file name in the mod root folder, for example preview.jpg. If it is omitted, the manager searches common names such as screenshot, preview, cover, and thumbnail.

### 7. Troubleshooting

- The mod is missing from the list: make sure it is inside the manager selected MOD folder, then click Refresh.
- The game folder is rejected: choose the folder that contains both tlou-i.exe and build\pc\main.
- The mod structure is rejected: confirm that the folder or archive contains build\pc\main.
- Installation fails: close the game, scan the game archives again, and refresh the mod list.
- The game behaves incorrectly: disable the most recently enabled mod and test with one mod at a time.
- You want to restore the original files: uncheck the mod and apply the changes again.
- The manager says another instance is running: close the existing manager window before starting it again.

**Full Changelog**: https://github.com/Vyaomo/TLOU-Mod-Manager/compare/v1.1.28...v1.1.46
