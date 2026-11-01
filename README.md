# Aeris Maven

Aeris Android SDK 的 Maven 制品仓库，供原生 App、React Native、Flutter、WebView 和 Unity 接入原生通信能力。

## 仓库配置

将以下地址加入宿主工程的依赖仓库配置，保留 `google()` 和 `mavenCentral()`：

```kotlin
maven {
    url = uri("https://raw.githubusercontent.com/zhangguozhong/aeris-maven/0.26.0-preview.2")
    content { includeGroup("com.aeris.sdk") }
}
```

## 原生依赖

```kotlin
implementation("com.aeris.sdk:aeris:0.26.0-preview.2")
```

最低 Android API `24`，使用 Java `17`。

按需选择 `aeris-react-native`、`aeris-web`、`aeris-flutter`、`aeris-unity`。RN/Flutter 插件通过 npm/pub.dev 安装后，由平台工具接入对应原生模块。

Unity 的 `aeris-unity-channel` 用作宿主的 `compileOnly` 契约；通道实现随 UnityLibrary 编译，宿主不要重复打包。

[完整接入说明](https://github.com/zhangguozhong/aeris-sdk#android原生依赖)。源码与许可证见 [Aeris](https://github.com/zhangguozhong/aeris-sdk)。
