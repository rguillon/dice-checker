# dice-checker

[![Release](https://img.shields.io/github/v/release/rguillon/dice-checker)](https://img.shields.io/github/v/release/rguillon/dice-checker)
[![Build status](https://img.shields.io/github/actions/workflow/status/rguillon/dice-checker/ci.yml?branch=main)](https://github.com/rguillon/dice-checker/actions/workflows/ci.yml?query=branch%3Amain)
[![codecov](https://codecov.io/gh/rguillon/dice-checker/branch/main/graph/badge.svg)](https://codecov.io/gh/rguillon/dice-checker)
[![Commit activity](https://img.shields.io/github/commit-activity/m/rguillon/dice-checker)](https://img.shields.io/github/commit-activity/m/rguillon/dice-checker)
[![License](https://img.shields.io/github/license/rguillon/dice-checker)](https://img.shields.io/github/license/rguillon/dice-checker)

A simple library to compute probabilities with dice rolls.


Dice objects can be created from a simple RPG-like string expression:


```python

from dice_checker import DiceD

Dice("D6")
Dice("2D8+1")
Dice("5D10-1D6-1")


```

```python

>>> from dice_checker import Dice
>>> roll = Dice("2D6+1")
>>> print(roll.distribution)
{3.0: 1.0, 4.0: 2.0, 5.0: 3.0, 6.0: 4.0, 7.0: 5.0, 8.0: 6.0, 9.0: 5.0, 10.0: 4.0, 11.0: 3.0, 12.0: 2.0, 13.0: 1.0}

```
