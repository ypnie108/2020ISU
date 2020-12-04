## 作業 No. 9 練習類別建構子的寫法, this()及this參考的使用, 封裝的實作
 
### 二維空間的Point類別
   - 實體變數成員(private等級):  int x,  int y
   - 建構子: 
      - 預設建構子//定在(0,0)位置
      - public Point(int x, int y)
      - public Point(int n) //定在(n,n)位置
   - 實體方法
	    - public void displayPoint() //顯示點的資訊
      - public void updatePoint(int x, int y) //更新x,y座標
      - private boolean checkPoint(int x, int y) //檢核點的座標 -> x,y必須在第一象限
   - 備註: 
      - 建構子及updatePoint() 中需要檢核x,y在第一象限
      - public Point(int n)建構子中利用public Point(int x, int y)來完成建構的邏輯

### 相關教學影片[連結](https://youtu.be/dyNwznzma0s)
   - 不知道如何開始着手的同學可以參考上面youtube影片.
