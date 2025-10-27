# vscode_extension
製作 vscode 套件

## 安裝製作工具
```
npm install -g yo generator-code
```

```
yo code
```
![這是圖片](/assets/img/yo_code.png)

#### 註冊 command
package.json  
![這是圖片](/assets/img/package.json.png)

extensin.js  
![這是圖片](/assets/img/extension.js.png)

#### 測試
1. 按 F5
2. 輸入剛剛註冊的 title 名稱 (Hello World)
![這是圖片](/assets/img/command.png)
3. 即可看到輸出結果
![這是圖片](/assets/img/result.png)

## 如何打包
#### 圖片打包方式
在 package.json 補上 repository (vsce 會自動推導圖片的絕對網址)
![這是圖片](/assets/img/repository.png)

#### 將 vscode 套件打包成.vsix
安裝打包工具
```
npm install -g vsce
```
進行打包
```
vsce package
```
![這是圖片](/assets/img/test.vsix.png)

## 如何使用 .vsix 
<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>P</kbd>
<br>
輸入 Extensions: Install from VSIX...
