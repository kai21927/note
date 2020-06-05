# TYPE SCRIPT
### TYPE SCRIPT簡介

>簡單來說TYPE SCRIPT就是**JS的進階版**(也稱為JS的超集合)，在TS檔案撰寫時能夠同時進行編譯，編譯出來的純JS可以運行在任何瀏覽器上。

### TYPE SCRIPT優點
* 引入強型別的概念，開發時能就能進行靜態的檢查，避免預期外的錯誤。
* 大幅增強的物件導向系統，增加程式碼的表達性，進而改善團隊維護成本與開發效率

### 為什麼需要學TYPE SCRIPT?
>目前來說前端框架日新月異，不論是套件、框架，有很大的機率會轉換成另一種形式，但像RxJS、ReactJS、Angular、VueJS等主流框架和套件都開始支援TS，學TS對於目前使用主流框架是有所幫助的。


### TYPE SCRIPT環境建置
1. 需先安裝Node.js
    https://nodejs.org/en/download/
2. 打開CMD，輸入指令安裝TYPE SCRIPT
    ```
    npm install -g typescript
    ```
>以下程式碼編輯器使用VS CODE做範例
### vscode配置ts文件自動轉換成js文件
1. 新建項目，生成tsconfig.json配置文件
    ```
    cd 目錄 tsc --init 
    ```
2. 開啟目錄內tsconfig.json檔修改JS輸出路徑
   >打開註解後將outDir:  " ./ "改成outDir:  " ./js "
   
   >編譯後的JS檔將會在根目錄底下的JS資料夾
3. VS CODE配置任務，運行任務
    * 點擊終端機。
    * 點擊執行工作
    * 選擇TSC監視

完成步驟後，寫TS檔程式碼同時會轉譯成./js檔供HTML引入用。

### TS指定型別時使用冒號( : )當未指定型別，TS也會進行型別推論，主動幫變數判別型別。
```
 let a:String = "記得用冒號"; //指定型別
 let a = "沒有冒號時"         //TS型別推論為字串
```
### 目前使用JS與TS上的差異

| 語言 |型別  | 差異 |
| ------ | ------ | ------ |
| JAVA SCRIPT | 弱型別 | 型別判讀上較為寬鬆 |
| TYPE SCRIPT | 強型別 | 型別判讀上較為嚴謹 |
開發大型專案時，在ts靜態編寫時就會辨識錯誤，並且提示錯誤在哪，會減少之後debug的時間。而JS在編寫時並不會出現錯誤，直到執行時才會出現錯誤，到時再來找尋錯誤，會增加debug的時間。
### 介紹VS插件quokka.js協助撰寫JS或TS時更加方便
    >按下Ctrl + Shift + P
    上方選擇quokka.js start on current file
可在VS CODE裡頭迅速查看console.log的結果。



  