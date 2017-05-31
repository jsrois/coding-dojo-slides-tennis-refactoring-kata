# Coding Dojos

#HSLIDE
## Why Coding Dojos?

#HSLIDE
## Why Coding Dojos?

- Deliverate Practice
- Focus on doing it perfectly, not getting it done

#HSLIDE
## Deliverate Practice
![etudes](music_etudes.jpeg)
![orchestra](https://blair.vanderbilt.edu/images/ensembles/orchestra.JPG)

#HSLIDE
## Deliverate Practice
![training_soccer](https://www.vigoe.es/media/k2/items/cache/7371c75eb67b3f9c2e0dcc9c27bb09c6_XL.jpg)

#HSLIDE
## Deliverate Practice
![dibujo_tec](https://i.ytimg.com/vi/tV7oMIKCGpo/maxresdefault.jpg)

#HSLIDE
##Don't Focus on Getting it Done. Focus on Doing It Perfectly.

#HSLIDE
# Testing

#HSLIDE
# When do we need tests?

#HSLIDE
## When do we need tests?

- When adding new features (TDD)
- Refactoring
- Catching Bugs

#HSLIDE
# Refactoring

#HSLIDE 
# Why refactoring?
![wtfs_minute](https://blog.codinghorror.com/content/images/uploads/2009/02/6a0120a85dcdae970b012877707a45970c-pi.png)

#HSLIDE
## Refactoring
_Changing the internal structure of code without changing its behavior_

#HSLIDE 
## Refactoring 
_**Improving** the internal structure of code without changing its behavior_ 

#HSLIDE 
## Refactoring 
_Improving the internal structure of code **without changing its behavior**_ 

#HSLIDE 
## Refactoring 
_Improving the internal structure of code **without breaking it**_

Tests tell us if we break it.


#HSLIDE 
## Tennis Refactoring Kata

- **You already have the tests in place**
- Start with the first version of the TennisGame
- Discuss what you don't like
- Change the code step by step

#HSLIDE
## Tennis Refactoring Kata
### 5': for setup

#HSLIDE
## Tennis Refactoring Kata
### 10': what is wrong with this code?

#HSLIDE
## Tennis Refactoring Kata
### PROBLEM: This code requires **domain** (business) knowledge

#HSLIDE
# Let's go! And remember:

> Don't Focus on Getting it Done. Focus on Doing It Perfectly

#HSLIDE
# Recap

#HSLIDE
#### Refactoring example: Tell, Don't Ask (OO)

#HSLIDE
#### Refactoring example: Tell, Don't Ask (OO)
> An object is a bundle of capabilities (Allen Holub)

#HSLIDE
#### Refactoring example: Tell, Don't Ask (OO)

Before: 

```python
def won_point(self, playerName):
    if playerName == self.player1Name:
      self.p1points += 1
    else:
      self.p2points += 1
```

#HSLIDE
### Refactoring example: Tell, Don't Ask (OO)

After:

```python
def won_point(self, name):
    player = self.get_player_by(name)
    player.won_point()
```
