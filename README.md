# 万能刷题通

基于 Capacitor 构建的 Android 刷题应用。

## 预构建 APK

预构建的 APK 文件位于 `outputs/万能刷题通.apk`。

## 环境要求

- Node.js 18+
- JDK 21 (如 Eclipse Adoptium JDK 21)
- Android SDK (compileSdk 36, targetSdk 34, minSdk 24)
- Gradle 8.14.3 (项目自带 gradle wrapper)

## 构建步骤

```bash
# 1. 安装依赖
npm install

# 2. 同步 Capacitor 到 Android 项目
npx cap sync android

# 3. 构建 APK
cd android
./gradlew assembleDebug
```

构建完成后，APK 文件位于：
```
android/app/build/outputs/apk/debug/app-debug.apk
```

## 技术栈

- Capacitor 8.x - 跨平台框架
- Android Gradle Plugin 8.13
- 纯 Web 前端 (HTML/CSS/JS) 内嵌 WebView

## 应用信息

- 包名：com.quiz.wanneng
- 应用名：万能刷题通
- 最低 Android 版本：7.0 (API 24)