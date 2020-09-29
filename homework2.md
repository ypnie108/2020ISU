## 作業 No. 2

### RGBA顏色格式
1. 參考wiki的關於RGBA的顏色格式的介紹:[連結](https://zh.wikipedia.org/wiki/RGBA)
1. 使用一個byte來儲存紅色RED成分, 一個byte來儲存綠色GREEN成分,  一個byte來儲存藍色BLUE成分, 一個byte來儲存透明度(ALPHA)成分
1. 一個byte數值使用全部正數的範圍(0-255)
1. ALPHA值若為0, 代表完全透明, 255代表完全不透明
1. 所以可以使用一個int型態(佔據4個bytes)的變數來儲存RED,GREEN,BLUE,ALPHA

### 定義一個代表顏色的類別 Rgba
1. 成員變數: int red, int green, int blue, int alpha
1. 建構子: 
   - Rgba(int c) : 參數 int c 的byte 1為RED成分, byte 2為GREEN成分, byte 3為BLUE成分, byte 4為ALPHA成分
   - Rgba(int r, int g, int b, int a)
   - Rgba(double r, double g, double b, double a)
   

