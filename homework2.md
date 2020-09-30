## 作業 No. 2

### 相關教學影片[連結](https://youtu.be/ZpgwTwMd7Nc)
   - 不知道如何開始着手的同學可以參考上面youtube影片.
   
### RGBA顏色格式
1. 參考wiki的關於RGBA的顏色格式的介紹:[連結](https://zh.wikipedia.org/wiki/RGBA)
1. 使用一個byte來儲存紅色RED成分, 一個byte來儲存綠色GREEN成分,  一個byte來儲存藍色BLUE成分, 一個byte來儲存透明度(ALPHA)成分
1. 一個byte數值使用全部正數的範圍(0-255)
1. ALPHA值若為0, 代表完全透明, 255代表完全不透明
1. 所以可以使用一個int型態(佔據4個bytes)的變數來儲存RED,GREEN,BLUE,ALPHA

### 定義一個代表顏色的類別 Rgba
1. 成員變數: int red, int green, int blue, int alpha
1. 建構子: 
   - Rgba(int c) 
      - 參數 int c 的byte 1為RED成分, byte 2為GREEN成分, byte 3為BLUE成分, byte 4為ALPHA成分
   - Rgba(int r, int g, int b, int a)
      - 需檢查r, g, b, a都介於 0-255 之間
   - Rgba(double r, double g, double b, double a) 
      - 參數為double型態, 代表每一個顏色成分的百分比(0.0到1.0)
      - 例如0.5等同於255*0.5=127
      - 需檢查r, g, b, a 都介於 0.0-1.0 之間
1. 成員方法:
   - void invertColor()
      - 反轉顏色
      - 透明度不需要改變
   - void setNonTransparent()
      - 設定成完全不透明
   - void displayColorButton()
      - 顯示顏色視窗
   - void java.awt.Color toColor()
      - 轉換成java.awt.Color物件
  
``` 

public static int pos=1;
public static int serial=1;

public Color toColor() {
	System.out.printf("red:%d, green:%d, blue:%d, alpha:%d\n", red, green, blue, alpha);
	return new Color(red, green, blue, alpha);
}

public void displayColorButton() {
	JFrame f = new JFrame();
	f.setLocation(pos += 300, 1);
	f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
	FlowLayout bl = new FlowLayout();
	f.setLayout(bl);
	f.setTitle("Color Frame: " + serial++);
	f.setSize(250, 250);
	JButton b = new JButton("Color");
	b.setFont(new Font("Arial", Font.PLAIN, 80));
	b.setPreferredSize(new Dimension(250, 250));
	b.setBackground(Color.BLACK);
	b.setForeground(toColor());
	f.add(b);
	f.setVisible(true);
}
```
   
### 主要類別: TestRgba

1. 定義 main()方法
   - 產生Rgba物件: 
      - Rgba r1 = new Rgba(128,128,0,128)
      - Rgba r2 = new Rgba(0.1,0.8,0.9,0.6)
   - 呼叫r1.displayColorButton()
   - 呼叫r2.displayColorButton()
   - 呼叫r2.setNotTransparent()
   - 呼叫r2.displayColorButton()
   - 呼叫r2.invertColor()
   - 呼叫r2.displayColorButton()
