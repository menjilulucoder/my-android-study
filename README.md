# Android 第一行代码学习笔记 (Ch01-Ch03)

## 第一章：Android 开发环境与项目结构
* **项目目录**：`app/src/main/java` 存放代码，`res` 存放资源（布局、图片、字符串），`AndroidManifest.xml` 是项目清单。
* **Logcat**：日志工具，分为 Verbose, Debug, Info, Warn, Error 五个级别，支持 Tag 过滤。

## 第二章：Kotlin 语言基础
* **变量**：使用 `val` 声明不可变变量（优先），使用 `var` 声明可变变量。
* **空指针检查**：通过 `?` 声明可为空，`?.` 安全调用，`?:` 空值合并。
* **语法糖**：`when` 表达式替代 switch，支持更灵活的逻辑判断。

## 第三章：Activity 活动组件
* **生命周期**：
    * `onCreate()`：初始化布局和数据。
    * `onStart()` / `onStop()`：可见与不可见切换。
    * `onResume()` / `onPause()`：交互与暂停切换。
    * `onDestroy()`：回收资源。
* **Intent**：
    * 显式 Intent：指定类名跳转。
    * 隐式 Intent：匹配 Action 跳转。
    * 数据传递：通过 `putExtra()` 传值。
* **启动模式**：standard（默认）, singleTop（栈顶复用）, singleTask（栈内唯一）, singleInstance（独立栈）。
