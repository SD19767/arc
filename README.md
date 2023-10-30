# Xcode 模擬器打不開 SDK does not contain 'libarclite' at the path
當更新 Xcode 後，Rosetta模擬器有時候會打不開。這是因為這幾次 Xcode 更新有瘦身，Rosetta 的模擬器不包含在安裝包裡。
<img width="705" alt="image" src="https://github.com/SD19767/arc/assets/125421319/4251d714-6a0f-4463-9a12-c4895e791ca8">

如圖，這個錯誤十分惱人。
SDK does not contain 'libarclite' at the path '/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/lib/arc/libarclite_iphonesimulator.a'; try increasing the minimum deployment target
# 步驟一，打開 Finder 並且搜尋預期找到檔案的路徑
<img width="691" alt="image" src="https://github.com/SD19767/arc/assets/125421319/0236aaf9-f0c0-4c91-860e-50f141a9093d">

<img width="702" alt="image" src="https://github.com/SD19767/arc/assets/125421319/4bb1131d-fe8c-473d-90e1-4a31bdc9e022">

我這邊搜尋的路徑是： 
```
/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr
```
找到 lib 的資料夾，看看有沒有arc 得資料夾，如果沒有，下載這個檔案，並且將裡面的資料貼上即可。

<img width="705" alt="image" src="https://github.com/SD19767/arc/assets/125421319/90facfe7-bf66-4498-93cf-ca93c297a5e8">
