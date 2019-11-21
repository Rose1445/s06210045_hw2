# 如何使用此程式

- 開發軟體環境
- 主程式位置

## 開發軟體環境

![image](https://jupyter.org/assets/nav_logo.svg)

  Jupyter Notebook 是一個建構於網頁應用程式的開源整合開發環境，允許資料科學團隊像是在筆記本計算一般地撰寫程式、顯示程式和視覺化輸出、支援 Markdown 標記語言與 LaTex 數學方程式的文字段落。
  
  其中 Ju 指的是 Julia 語言、py 指的是 Python 語言以及 r 指的是 R 語言。
  
  而Project Jupyter 由 IPython 專案發跡，主要以支援 Python 語言與 Python 虛擬環境為主。

### 下載與安裝
Anaconda 提供完整解決方案，是資料科學團隊的首選推薦，除了 Python 3 直譯器，它還具備諸多特色：
  - 模組與虛擬環境的管理器 conda
  - 多樣化的整合開發環境，包含 Jupyter Notebook、Jupyter Lab、Spyder 與 RStudio
  - 預先安裝好 Python 資料科學應用模組，包含 NumPy、pandas、matplotlib 與 sklearn 等
  
#### 如欲安裝，可前往 Anaconda 下載頁面，依照不同作業系統點選對應的 Python 3 安裝檔。

![image](https://miro.medium.com/max/3590/1*LVQLaIqcWFcBopPk5LQ_Bg.png)
  
## 主程式位置

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


- 打造 Jupyter Notebook 資料科學環境
  - https://medium.com/datainpoint/jupyter-kernels-3151a6408bab
  
- 給自學者的Python教學(7)：字串(String)
  - https://medium.com/@ChunYeung/%E7%B5%A6%E8%87%AA%E5%AD%B8%E8%80%85%E7%9A%84python%E6%95%99%E5%AD%B8-7-%E5%AD%97%E4%B8%B2-string-1fa93a9aa471

- Python strip()方法
  - https://www.runoob.com/python/att-string-strip.html
  
- Bubble Sort & Merge Sort
  - https://www.runoob.com/python3/python-bubble-sort.html
  - https://www.runoob.com/python3/python-merge-sort.html
