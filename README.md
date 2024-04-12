import pygame
import random

# Initialize Pygame
pygame.init()

# Set up game window
window_x = 720
window_y = 480
game_window = pygame.display.set_mode((window_x, window_y))
pygame.display.set_caption('Snake Game')

# Initialize snake position and other variables
snake_position = [100, 50]
snake_body = [[100, 50], [90, 50], [80, 50]]
fruit_position = [random.randrange(1, (window_x // 10)) * 10, random.randrange(1, (window_y // 10)) * 10]
fruit_spawn = True
direction = 'RIGHT'
snake_speed = 15

# Function to display the score
def show_score(choice, color, font, size):
    score_font = pygame.font.SysFont(font, size)
    score_surface = score_font.render('Score: ' + str(score), True, color)
    game_window.blit(score_surface, (5, 5))

# Main game loop
while True:
    # Game logic here...
    # (Refer to the full code in the GeeksforGeeks link below)

    pygame.display.update()
    fps.tick(snake_speed)
