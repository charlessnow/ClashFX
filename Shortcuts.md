 # 全局快捷键

ClashFX的全局快捷键是通过支持 AppleScript，并以系统的 Automator 程序调用 AppleScript 来完成全局快捷键的实现。

ClashFX目前仅支持以下功能的AppleScript

1.  打开（关闭）系统代理
2.  切换出站模式

## 通过 Automator 创建全局快捷键

[Mac新建全局快捷键](https://www.jianshu.com/p/afee9aeb41a8)

## 可用的 AppleScript 

你可以在这里选择你需要的 AppleScript 代码，以此创建你需要的快捷键。 

**以下示例代码为ClashFX程序。如果你正在用ClashFX Pro，那么请将ClashFX替换为 ClashFX Pro**

---

打开（关闭）系统代理

`tell application "ClashFX" to toggleProxy`

切换出站模式为全局代理

`tell application "ClashFX" to proxyMode 'global'`

切换出站模式为直连

`tell application "ClashFX" to proxyMode 'direct'`

切换出站模式为规则代理

`tell application "ClashFX" to proxyMode 'rule'`

## 已知缺陷

1. 无法直接在桌面使用快捷键，你需要进入任意程序中才能启动快捷键
   
2. 在任何程序中第一次启用该快捷键都要点击一次确认授权才能启动快捷键