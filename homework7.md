## 作業 No. 7

### 延續`作業6`所寫的電子商務系統, 根據`ShoppingCart`物件內容來產生Order物件
### ShoppingCart 類別:
   - 增加`exportItems()`方法: 用來匯出ShoppingCart物件中所包含的ProductItem[]陣列
   - 匯出ProductItem[]陣列時, 需根據實際的ProductItem數目(記錄在itemCount成員變數中)來產生這個陣列
   - 可以利用System類別的arraycopy()[方法](https://docs.oracle.com/javase/7/docs/api/java/lang/System.html#method_summary):
       - public static void arraycopy(Object src,int srcPos,Object dest,int destPos,int length)
### Order 類別:
   - 類別圖如右:
