# 什么是 MAplus

MAplus（全称 Mapping Assistant plus），是利用 Virtools（简称 vt）内建的 Action 开发的一套工具，其运行方式与 Virtools 自带的 Actions 相同。这套工具对 Virtools 内许多繁琐操作进行了简化，以 VSL 脚本的方式进行半自动化批量操作。

此工具包目前涵盖了物件操作，网格操作，归组辅助，灯光辅助，命名辅助共 5 个方面，大多数情况下能为 vt 内操作节省大量繁琐操作，减少出错率；在使用熟练之后可以使 vt 内操作效率大幅提高。

不过， vt 内使用 Action 进行的操作是无法撤销的。尽管大部分时候错误操作不会造成过于严重的损失，还是建议制图者养成随手保存的习惯。

## 安装

### 基本内容

MAplus 所包含的项目列表如下:

| 项目名称                  | 项目类型     | 基本描述                            |
| ------------------------- | ------------ | ----------------------------------- |
| [B_3DEntity](B_3DEntity)  | 文件夹       | 物件操纵类                          |
| [B_Group](B_Group)        | 文件夹       | 归组辅助                            |
| [B_Light](B_Light)        | 文件夹       | vt 内灯光辅助                       |
| [B_Mesh](B_Mesh)          | 文件夹       | 网格工具                            |
| [B_Name](B_Name)          | 文件夹       | 命名工具                            |
| [Virtools](Virtools)      | 文件夹       | vt 原版 Actions（已进行防重名微调） |
| ActionEditorInterface.ini | ini 配置文件 | 配置文件                            |
| ActionEditorList.ini      | ini 配置文件 | 配置文件                            |

### 如何安装

MAplus 安装很方便 ~~（真的）~~。下面给出了最方便的安装方法：

1. 关闭 vt
2. 找到 vt 根目录下 Actions 文件夹，并进入
3. 删去其中所有文件夹、文件
4. 将 MAplus 内的所有文件夹及配置文件放入
5. 启动 vt ，此时应已安装完毕并可供使用

```
除此以外，release 还放出了内置 MAplus 的完整 Virtools 3.5。也可直接下载使用。
预制的 vt 中关于 MAplus 的部分配置已经调整至一般制图党的需求，并内置了最新的 MAplus。
若不想手动安装可以使用此整合版。但安装新的 vt 需要更改文件默认打开方式，否则在打开 CMO 文件时系统依旧会调用原有的 vt 。
```

## 基本使用方法

在 vt 内 `3D layout` 或 `Level Manager` 界面单击鼠标右键，`Actions` 选项内选择需要调用的 Action 即可。

Actions 的调用与是否在物件上点击右键无关，所以不需要在物件上点右键也能将选择的物件正常操作。不在物件上点击右键可以使右键菜单不过于冗长，一定程度上提高了使用 Actions 的使用效率。

## 设置快捷键

在 Virtools 中选择 `Editors` – `Action Manager` 可以设置快捷键。

在任意 Action 的名称上点击右键，选择 `Edit Keyboard Shortcut` 即可设置快捷键。

快捷键设置规则：

```
Control/Shift/Alt 中的一个 + F1 至 F12 任意一个功能键 (除了 Alt + F4)
```

注意，第一次打开 `Action Manager` 时不会出现新安装的 Actions，此时推荐手动删去所有的选项卡（选项卡是指 `Import all Actions` 按钮右边的选项卡，可右键选择 `Remove Tab` ，若不删去会导致选项卡重复添加），再点击 `Import all Actions` 按文件目录导入全部 Actions 。

成功导入后应出现总计 9 个选项卡。若有重复删去即可。

下面是推荐设置快捷键的 Actions：

-   Align2
-   Splice
-   FastSplice
