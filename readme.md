1. pip install manim
2. touch rotating_square.py // just a random file
3. sample code => 
```
    from manim import *
    class RotatingSquare(Scene):
    def construct(self):
        square = Square(side_length=2, color=BLUE)
        self.play(Create(square))
        self.play(Rotate(square, angle=PI/2))
        self.play(square.animate.shift(LEFT * 2))
        self.wait(1)
```

4.manim -pql rotating_square.py RotatingSquare
