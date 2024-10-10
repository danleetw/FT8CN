# FT8TW

感謝BG7YOZ跟N0BOY
寫出了一個如此有趣又方便的程式，大幅減少了我在山上做SOTA的設備數量，以及纜線的數量，
因為除了不可少的無線電機、電池、天線以外，可以少帶電腦以及一堆雜亂的線材，在爬山的過程減少了許多重量，在開始架設SOTA電台時，也節省了很多步驟，
反之，在遇到下雨刮風等天候不佳的情況時，能盡可能地用最快速度把裝備整理好，丟回登山背包中，也可以避免體溫流失太多以及裝備收潮的風險，
讓我再次感謝二位。

我的立場是儘可能使用原來的FT8CN版本，這個地方的FT8TW版本，則是一些我的概念驗證區域，如果驗證可行，我還是會提交我的資訊給BG7YOZ。
畢竟我沒有想要喧賓奪主喔，如果需要正式的、完整的FT8CN版本，可以參考 https://github.com/N0BOY/FT8CN ,
Check [Releases](https://github.com/N0BOY/FT8CN/releases) to download the latest apk file.

```
DE BV6LC
2024/10/10
```

2024/10/10 FlexRadioInfoFragment.java 
```
這個錯誤來自於 Android 的 Fragment 使用過程中，當你在觀察 LiveData 時，應該使用 getViewLifecycleOwner() 來作為 LifecycleOwner。這樣可以確保 LiveData 觀察者在 Fragment 的 view 銷毀時自動移除，避免內存洩漏或意外行為
```

避免與目前執行版本一樣，以致無法安裝或弄壞正常版本(改applicationId)
app\build.gradle
app\src\main\AndroidManifest.xml
app\src\main\res\drawable\ft8cn_icon.png



調整繁體地區說明(不知是否造成簡繁體顯示錯誤修改測試)
app\src\main\country_en2hk.dat
app\src\main\java\com\bg7yoz\ft8cn\callsign\CallsignDatabase.java
app\src\main\java\com\bg7yoz\ft8cn\callsignCallsignFileOperation.java

調整部分翻譯
app\src\main\res\values\*\string.xmls


翻轉藍芽設備時，造成藍牙中斷，輸入為0.5
app\src\main\java\com\bg7yoz\ft8cn

移除音量調整，在S24手機會造成閃退
app\src\main\java\com\bg7yoz\ft8cn\grid_tracker


新增GPS校正時間
app\src\main\assets\ConfigFragment.java

新增網頁本手動新增關注呼號
app\src\main\java\com\bg7yoz\ft8cn\html
app\src\main\java\com\bg7yoz\ft8cn\GeneralVariables
