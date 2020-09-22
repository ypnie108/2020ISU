### 定義一個長方形(Rectangle)類別 
1. 成員變數:
    - 長: public int height
    - 寬: public int width 
1. 建構子:
    - public Rectangle()
    - public Rectangle(int h, int w)
1. 方法:
    - 計算面積: public int calculateArea()
    - 列印資訊(列印長寬面積等資訊): public void printInformation()
1. 程式註解(javadoc)
    - 利用javadoc產生java html註解文件
    
### 定義主要類別(RectangleTest)類別  
1. main()方法
    - 產生第一個Rectangle物件r1
        - 呼叫Rectangle()
    - 產生第二個Rectangle物件r2
        - 呼叫Rectangle(int h, int w)
    - r1.printInformation()
    - r2.printInformation()
