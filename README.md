# 大字語音計算機

專門給高齡使用者的 Android 離線計算機。

## 第一版功能

- 超大數字顯示
- 超大按鍵
- ＋、－、×、÷
- AC 全部清除
- 退格
- 小數點
- 等於
- Android 原生 TTS
- 按數字會朗讀
- 按運算符號會朗讀
- 按「＝」會朗讀答案
- 完全離線計算
- AndroidManifest **沒有 INTERNET 權限**
- GitHub Actions 自動編譯 Debug APK

## 離線語音

App 本身不需要網路。

若手機已安裝「中文（台灣）」的離線 TTS 語音資料，朗讀也可以完全離線。
若手機沒有離線語音資料，計算功能仍可正常使用。

## GitHub Actions

每次 push 到 `main` 後，GitHub Actions 會自動編譯 APK。

完成後：

1. 進入 GitHub Repository
2. 點 `Actions`
3. 點最新一次 `Build Android APK`
4. 往下找到 `Artifacts`
5. 下載 `senior-calculator-debug-apk`
6. 解壓縮後安裝 `app-debug.apk`

## 技術

- Java
- Android 原生 UI
- Android 原生 TextToSpeech
- 無第三方函式庫
- minSdk 23
- targetSdk 35
