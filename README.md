# SystemX - 基于 Shizuku 的系统优化助手

## 项目简介

SystemX 是一个 Android 应用，利用 Shizuku 项目，允许用户在 无需 root 的前提下访问部分系统级 API，实现诸如：

查看 App 使用时间和次数

一键清理缓存和停止后台应用

管理 App 权限状态（通过 AppOps）

后续扩展更多系统优化功能

## 技术栈

Java（主要语言）

Android SDK (targetSdkVersion 34)

Shizuku API

AIDL / Binder 通信

UsageStatsManager / AppOpsManager / ActivityManager 等系统服务

## 项目模块

### App 使用统计

获取前台使用时长、启动次数、包名等

用图表展示使用最多的应用

### 后台进程管理

使用 Shizuku 获取 ActivityManager 并终止指定 app 后台

可视化列表显示正在运行的应用

### 缓存清理模块

使用隐藏 API 清除应用缓存（需系统权限或 ADB 权限）

选中目标 App 后点击清除

### 权限控制器
使用 AppOpsManager 获取应用权限状态

开关位置权限、通知权限等（兼容不同 API 级别）
