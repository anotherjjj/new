# new
import pygame
from pygame.draw import *

pygame.init()

FPS = 30
screen = pygame.display.set_mode((400, 400))

rect(screen, (200, 200, 200), (0, 0, 400, 400))
circle(screen, (255,100,10), (200, 400), 100)
circle(screen, (200,190,140), (200, 230), 90)
circle(screen, (0,0,0), (170, 225), 16, 1)
circle(screen, (0,255,255), (170, 225), 15)
circle(screen, (0,0,0), (170, 225), 5)
circle(screen, (0,0,0), (230, 225), 16, 1)
circle(screen, (0,255,255), (230, 225), 15)
circle(screen, (0,0,0), (230, 225), 5)



pygame.display.update()
clock = pygame.time.Clock()
finished = False

while not finished:
    clock.tick(FPS)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            finished = True

pygame.quit()
