# 如何使用此程式

- 開發軟體環境
- 主程式位置

## 開發軟體環境

![image](https://i.imgur.com/5MPeamM.png)

  要先在電腦上安裝 Java SDK 和 Eclipse IDE 兩套軟體。之後使用 Eclipse IDE 整合開發環境在上面建立 Java 專案，撰寫 Java 程式碼，將 Java 檔編譯成 class 檔，後直接將運行過程和結果輸出在資訊視窗中。

### 下載與安裝
#### 安裝 Java SDK

![image](https://i.imgur.com/FwQDKpO.jpg)
  - 可以 Goolge 搜尋 「Java SE Development Kit 8」，即可以找到目前官方最新版本。
  - 官方連結：https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

安裝 Eclipse IDE
  - 連結：https://www.eclipse.org/
  
#### 主程式位置

前面將數據都處理好之後

以下為主要運算之程式碼:

count = 0

  - count用於統計字符串裡某個字符出現的次數。 可選參數為在字符串搜索的開始與結束位置

for i in range(0,len(a)):

  - len為返回列表元素個數

    for j in range(i+1,len(a)):
    
        print(i,j)
        
        if(a[i]>a[j]):
        
            count +=1
            
  - 此迴圈讓前一個數一一跟後面的數去做比較

## 參考資料


- 【從零開始學 Java 程式設計】安裝 JAVA 開發軟體
  - http://tw-hkt.blogspot.com/2019/03/java.html
  
- 給自學者的Python教學(7)：字串(String)
  - https://medium.com/@ChunYeung/%E7%B5%A6%E8%87%AA%E5%AD%B8%E8%80%85%E7%9A%84python%E6%95%99%E5%AD%B8-7-%E5%AD%97%E4%B8%B2-string-1fa93a9aa471

- Python strip()方法
  - https://www.runoob.com/python/att-string-strip.html
  
- Bubble Sort & Merge Sort
  - https://www.runoob.com/python3/python-bubble-sort.html
  - https://www.runoob.com/python3/python-merge-sort.html
