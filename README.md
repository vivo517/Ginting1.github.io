import turtle

# Setup layar
screen = turtle.Screen()
screen.bgcolor("white")

# Setup turtle
pen = turtle.Turtle()
pen.shape("turtle")
pen.color("red")
pen.speed(5)
pen.width(3)

# Fungsi untuk menggambar hati
def draw_heart():
    pen.begin_fill()
    pen.fillcolor("red")
    pen.left(50)
    pen.forward(133)
    pen.circle(50, 200)
    pen.right(140)
    pen.circle(50, 200)
    pen.forward(133)
    pen.end_fill()

# Pindahkan turtle ke posisi awal
pen.up()
pen.goto(0, -50)
pen.down()

# Gambar hati
draw_heart()

# Sembunyikan turtle
pen.hideturtle()

# Tutup layar saat diklik
screen.exitonclick()
