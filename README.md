# LiterarySimilarityComparison
碩士圖書館專案-文獻AB相似比對系統(Literary-Similarity-Comparison)

## 實作目的
在碩士期間，<br>
因教授為圖書館館長，有論文參考文獻可供分析，<br>
應需求研究參考文獻之間的相似度比對，<br>
額外加強對Python程式語言的NLP應用。<br>

## 設計理念與技術
使用WEB網頁應用程式的方式來製作專案，<br>
使用者將兩篇論文中的參考文獻，分別貼入應用程式中的textarea控制項，<br>
應用程式會自動將兩篇參考文獻做排序整理，<br>
分析完成後會顯示參考文獻之間的相似度分析結果與圖表可供參考。<br>
- HTML+CSS
- Bootstrap CSS Framework
- 原生JavaScript
- ChartJS
- Flask
- Fetch
- Jieba
- TF-IDF
- Jaccard Similarity


## 主要實作功能
實作功能包含分析兩篇論文中的參考文獻，<br>
首先將上傳的參考文獻做排序清理，接著透過Jieba將參考文獻斷詞，<br>
使用TF-IDF將斷詞後的文字轉為向量，最後使用Jaccard Similarity將參考文獻做逐行分析，<br>
之後使用ChartJS將結果以圖表方式呈現。<br>
- 參考文獻AB Test分析 (Jieba->TF-IDF->Jaccard Similarity)
- 分析處理進度條顯示(UUID)
- MVVM前後端分離架構
- 排序使用者上傳之參考文獻
- 整體文獻相似度比對與視覺化BI儀表板分析
- 逐行文獻相似度比對與視覺化BI儀表板分析
- 文獻相似度內容即時比對
- 疑似高相似度文獻提醒顯示

## 相關程式畫面
### 登入註冊<br>
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/7.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/8.png">
<br>

### 使用者介面<br>
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/1.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/2.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/3.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/4.png">
<br>

### 管理者介面<br>
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/5.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/6.png">
<br>

## 製作過程與困難點
在實作該專案的過程中，有嘗試想要實際讓資料庫可以被外部來連接，<br>
達成實際直接遠端資料庫的功能，<br>
所以在網路這方面有另外研究了關於虛擬伺服器的功能，<br>
讓實作出來的程式也能透過外部裝置來進行連線。
