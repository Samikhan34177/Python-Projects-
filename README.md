# Band Name Generator Project

import random

# Predefined word lists
adjectives = ["Awesome", "Terrible", "Fantastic", "Super", "Good", "Bright", "Swift", "Bold", "Creative", "Golden", "Cool", "Lucky"]
nouns = ["Pineapple", "Tiger", "Elephant", "Lion", "Haven", "Sphere", "Venture", "Edge", "Pulse", "Quest", "Forge"]
verbs = ["Rise", "Shine", "Grow", "Bloom", "Thrive"]
adverbs = ["Quickly", "Slowly", "Gently", "Vigorously"]

# Functions to generate brand names:

def generate_brand_names(num_names=5):
    brand_names = []
    for _ in range(num_names):
        adj = random.choice(adjectives)
        noun = random.choice(nouns)
        verb = random.choice(verbs)
        adv = random.choice(adverbs)
        brand_names.append(f"{adj} {noun} {verb} {adv}")
    return brand_names

# Generate and display brand names

print("Welcome to the Simple Brand Name Generator!")
num_names = int(input("How many brand names would you like to generate? "))

# Generate and print the names:
print("\nHere are your brand name:")
for name in generate_brand_names(num_names):
    print(f"- {name}")

# How It Works
The code uses two lists: adjectives and nouns.
It randomly picks one word from each list and combines them to form a brand name.
The user can specify how many names they want to generate.

# Example Output
# Input:

How many brand names would you like to generate? 5

# Output:

Here are your brand names:
- BrightHaven
- CoolEdge
- SwiftQuest
- BoldPulse
- CreativeSphere
