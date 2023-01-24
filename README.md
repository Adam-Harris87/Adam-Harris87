### Hi there 👋

- This is a work in progress

- 🔭 I’m currently working on the Data Science program at Codeup
- 🌱 I’m currently learning SQL, Python, Tableau, Machine Learning and more
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

Lets play rock, paper, scissors!

```python
import random

def convert_choice(choice):
    # convert player choice to a number
    if str.lower(choice) == 'rock': return 0
    elif str.lower(choice) == 'paper': return 1
    elif str.lower(choice) == 'scissors': return 2
    else: print('Invalid choice')
        
def convert_comp_choice(choice):
    # convert computer choice to rock, paper or scissor
    if choice == 0: return 'Rock'
    elif choice == 1: return 'Paper'
    else: return 'Scissors'

def rps(choice): # play rock, paper, scissors
    # get a random integer
    comp_choice = random.randint(0,2)
    player_choice = convert_choice(choice)
    comp = convert_comp_choice(comp_choice)
    # check who won
    if comp_choice == player_choice:
        print(comp + ', Tie')
    elif (player_choice == 0 and comp_choice == 1) | \
        (player_choice == 1 and comp_choice == 2) | \
        (player_choice == 2 and comp_choice == 0):
        print(comp + ', You lose')
    else: print(comp + ', You win')
```
