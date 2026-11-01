# Aeris Android Maven

Aeris Android预览制品，固定版本`0.26.0-preview.1`。仅用于自定义Maven仓库，不声明Maven Central发布或namespace所有权。源码与MIT许可证见 [aeris-sdk](https://github.com/zhangguozhong/aeris-sdk/tree/0.26.0-preview.1)。

```kotlin
maven { url = uri("https://raw.githubusercontent.com/zhangguozhong/aeris-maven/0.26.0-preview.1") }
implementation("com.aeris.sdk:aeris:0.26.0-preview.1")
```

按需选择aeris-react-native/aeris-web/aeris-flutter/aeris-unity。aeris-unity-channel仅供宿主compileOnly，运行时唯一实现由UnityLibrary提供。已发布版本与tag不覆盖；release-manifest.json记录源码及制品SHA256。详细接入与预览验收边界见源码仓库README。
