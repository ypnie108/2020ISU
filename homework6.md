## 作業 No. 6

### Part I : 根據物件導向分析設計的類別圖(Class Diagram)及類別之間的關係, 定義類別及旗下的成員變數, 建構子, 成員方法等
   - 這個練習是接續課堂上介紹的電子商務系統中已經定義的Product, ProductItem, Customer, Order等類別, 加入ShoppingCart(購物車)的類別 
   - 參考![類別關係圖](EC_new.png)
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
         - public void addItem(ProductItem i): 加入ProductItem, 須過濾重複加入的ProductItem
         - public void removeItem(ProductItem i) : 移除ProductItem, 須確認ProductItem有在裡面再做移除
         - public int calculateTotalPrice() : 計算總價格
         - public void printInformation() : 列印購物車資訊
      - 靜態(static)方法: 
         - calculateShoppingCartId(): 產生ShoppingCard id數值(等於Customer id)
	 
### Part II : 
         
