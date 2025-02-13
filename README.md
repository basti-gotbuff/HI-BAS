import turtle

# Set up the screen
screen = turtle.Screen()
screen.bgcolor("white")

# Create a turtle named "flower"
flower = turtle.Turtle()
flower.shape("turtle")
flower.color("red")
flower.speed(10)

# Function to draw a petal
def draw_petal():
    flower.circle(100, 60)
    flower.left(120)
    flower.circle(100, 60)
    flower.left(120)

# Draw the flower
for _ in range(6):
    draw_petal()
    flower.right(60)

# Draw the stem
flower.color("green")
flower.right(90)
flower.forward(300)

# Hide the turtle and display the window
flower.hideturtle()
turtle.done()
