## Turtle sample 

```
import ch.aplu.turtle.*;
import java.awt.Color;

public class FirstTurtle {

	public static void main(String[] args) {

		Turtle t1 = new Turtle();
		t1.setColor(Color.BLUE).setPenColor(Color.BLACK);
		t1.setPos(-50, 50); // center is the (0,0)
		t1.setLineWidth(2.0);
		for (int i = 0; i < 4; i++) {
			t1.forward(100);
			t1.left(90);
		}

		Turtle t2 = new Turtle(t1, Color.gray);
		t2.speed(25).penUp();
		t2.heading(90);
		t2.forward(50);
		t2.setFillColor(Color.ORANGE);
		t2.fill();
		// t2.hideTurtle();

		Turtle t3 = new Turtle(t1);
		t3.setColor(Color.RED).setLineWidth(2.0);
		t3.setPos(50, -50);
		for (int i = 0; i < 3; i++) {
			t3.right(120);
			t3.forward(80);
		}

		Turtle t4 = new Turtle(t1, Color.magenta);
		t4.heading(270);
		t4.penUp();
		t4.forward(50);
		t4.right(90);
		t4.label("Hello");

		Playground pg = t1.getPlayground();
		System.out.println("烏龜數量:" + pg.countTurtles());

	}

}
```
