import turtle
import colorsys

# Configuración inicial
turtle.speed("fastest")
turtle.bgcolor("white")
turtle.title("Girasol Amarillo")

# Dibujo del tallo verde
turtle.penup()
turtle.goto(0, -200)
turtle.pendown()
turtle.color("green")
turtle.pensize(5)
turtle.setheading(90)
turtle.forward(200)

# Dibujo de los pétalos amarillos
num_petals = 12
for _ in range(num_petals):
    turtle.color("yellow")
    turtle.begin_fill()
    turtle.circle(50)
    turtle.end_fill()
    turtle.right(360 / num_petals)

# Ocultar la tortuga y mostrar el dibujo
turtle.hideturtle()
turtle.done()

