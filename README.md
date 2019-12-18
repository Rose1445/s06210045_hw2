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

#### 安裝 Eclipse IDE
  - 連結：https://www.eclipse.org/
  
## 主程式位置

  - BF法

  // 取得使用者輸入的整數
		 		Scanner scanner=new Scanner(System.in);
		 		// 輸入此次作業指定Rod Length值
		 		System.out.print("Rod length: ");
		 		int n=scanner.nextInt();
		 		// 輸出Maximum revenue
		 		System.out.println("Maximum revenue: "+BruteForceRodcutting(Price,n));
  // 雙層循環建立r和s存入切割數點，以及Maximum revenue
	static int[] s=new int[100];
	static int BruteForceRodcutting(int price[],int n)
	// Bruteforce 暴力法: 列出每種切割方案，比較出Maximum revenue
	// 所需時間T=O(2^n)
	{
		if(n==0)
			{
				// 無法切割: return 0
				return 0;
			} 
		else
		{
			int  q=Integer.MIN_VALUE;  // q無窮小
			for(int i=1;i<=n;i++)
			{
				// 取q以及已分割求得的價值中取最大值
				q=Math.max(q, price[i-1] + BruteForceRodcutting(price, n - i));
			}
			return q;
		}
	}
   #### 以上為主要程式內容

  - BD法

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
