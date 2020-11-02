## 作業 No. 7

### 延續`作業6`所寫的電子商務系統, 根據`ShoppingCart`物件內容來產生Order物件
### ShoppingCart 類別:
   - 增加`exportItems()`方法: 用來匯出`ShoppingCart`物件中所包含的`ProductItem[]`陣列
   - 匯出`ProductItem[]`陣列時, 需根據實際的`ProductItem`數目(記錄在`itemCount`成員變數中)來產生這個陣列
   - 可以利用`System`類別的`arraycopy()`[方法](https://docs.oracle.com/javase/7/docs/api/java/lang/System.html#method_summary):
       - public static void arraycopy(Object src,int srcPos,Object dest,int destPos,int length)
### Order 類別:
   - `Order`類別圖如右![類別圖](orderClassDiagram.png):
