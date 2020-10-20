## 作業 No. 6

### 根據物件導向分析設計的類別圖(Class Diagram)及類別之間的關係, 定義類別及旗下的成員變數, 建構子, 成員方法等
   - 這個練習是接續課堂上介紹的電子商務系統中已經定義的Product, ProductItem, Customer, Order等類別, 加入ShoppingCart(購物車)的類別
   - ShoppingCart(購物車)的類別包含的內容:
      - 成員變數: 
         - public long id;
	      - public Customer customer;
	      - public ProductItem[] items;
	      - public int itemCount; //用來記錄產品項目數量
	      - public int totalPrice;
      - 建構子:
         - public ShoppingCart(Customer c); 
         - 傳入Customer參數, 以Customer的id作為ShoppingCart的id
         - items = new ProductItem[10]; // 最多 10 個 Product items
      - 成員方法:
         - public void addItem(ProductItem i)
         - public void removeItem(ProductItem i)
         - public int calculateTotalPrice()
         - public void printInformation()
         
