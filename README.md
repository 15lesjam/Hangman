# Hangman

#Import random element for future use
import random
#This program will pick a random word from the numerous lists
#Set number of games to 0 to begin with
num_games = 0

#Set up lists of words for animals
animal_list1 = ["aardvark", "beaver", "caterpillar", "echidna", "flounder"]
animal_list2 = ["giraffe", "hyena", "iguana", "jackal", "komodo dragon"]
animal_list3 = ["lobster", "maine coon", "newt", "otter", "poison dart frog"]
animal_list4 = ["quail", "rattlesnake", "shrimp", "tawny owl", "umbrella bird"]
animal_list5 = ["vulture", "weasel", "xray tetra", "yorkshire terrier", "zebra"]

#Set up lists of words for food items. (Will leave it at this for now)
food_list1 = ["apple", "bacon", "caramel", "dorito", "egg"]
food_list2 = ["fish", "ice cream", "jelly", "kit kat", "lemon"]
food_list3 = ["marshmallow", "noodles", "oranges", "pickle", "raspberry"]
food_list4 = ["spaghetti", "tiramisu", "water melon"]

#Make a list to contain these categories
category_list = [animal_list1, animal_list2, animal_list3, animal_list4, animal_list5, food_list1, food_list2, food_list3, food_list4]

#Create function that picks a random category, then a random word from it
def get_word():
    randomCategory = random.choice(category_list)
    word = random.choice(randomCategory)
    print(word)

get_word()

