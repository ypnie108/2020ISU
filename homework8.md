## 作業 No. 8

## Part I:
### 延續`作業6`所寫的電子商務系統, 在`Customer`類別中加入客戶登入密碼的屬性並可以產生預設的隨機密碼
   - 新增成員變數`password` 
      - 宣告方式: `public int password`
   - 新增static的方法`generateRandomPassword()`產生預設的隨機密碼
      - 宣告方式: `public static int generateRandomPassword()`
      - 預設產生7碼的數字密碼(介於 1000000 到 9999999)
      - 可以利用`Math.random()` static方法: 會回傳一個介於`[0,1.0)` 的double型態的亂數, 然後轉換到介於`[1000000,9999999]`之間的整數
   - 在`Customer`建構子中加入指定密碼的敘述(亦即將`generateRandomPassword()`的回傳內容指定給`password`成員變數)
   - 新增成員方法`getPassword()` : 回傳`password`
   - 主要類別`CustomerTest`中的`main()`中產生`Customer`物件, 取得其預設的`password`並列印顯示在銀幕上
 
## Part II:
### 將作業4中使用`阿基米德的圓內接正多邊形`來計算圓周率的演算內容變成Circle類別的一個static方法
   - public static double calculatePi(int n)
