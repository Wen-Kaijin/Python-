from turtle import *
from random import *

from setuptools import setup

#雪花函数
def drawSnow():
    hideturtle()
    pensize(2)
    #雪花数量
    for i in range(200):
        r, g, b = random(), random(), random()
        pencolor(r, g, b)
        penup()
        setx(randint(-350, 350))
        sety(randint(1, 270))
        pendown()
        dens = randint(8, 12)
        snowisze = randint(10, 14)
        for j in range(dens):
            forward(snowisze)
            backward(snowisze)
            right(360 / dens)

#地线函数
def drawGround():
    #地线数量
    for i in range(100):
        pensize(randint(5, 10))
        x = randint(-400, 350)
        y = randint(-280, -1)
        r, g, b, = -y / 280, -y / 280, -y / 280
        pencolor((r, g, b,))
        penup()
        goto(x, y)
        pendown()
        forward(randint(40, 100))

tracer(False)
bgcolor('black')
drawSnow()
drawGround()
done()
