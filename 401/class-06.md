# Random, Risk, and Big O

## Random module in python

```python
import random

# random integer 1-5
print random.randint(0,5)

# random flotaing point value 0-1
print random.random()

#random floating poing number 0-100
print random.random() * 100

# random element in a list
print random.choice( [item1, item2, item3, etc] )
```

These are some of the basics. There are a bunch of other methods for seeding random values and also getting differing distributions of random values in varying ranges. See the [documentation](https://docs.python.org/3/library/random.html)

## Risk analysis

There are several stages of risk analysis

1. Risk Identification
   * Business risks - come from your business or customer rather than from your project
   * Testing risks - be aware of your testing limitations and methods
   * Premature Release risks - be aware of implications of releasing buggy software
   * Software risks - be aware of your development process
2. Risk Assessment
   * Forecast problems
   * Estimate losses
   * Have an action plan
   * Learn from unwanted scenarios to avoid future consequences
3. Perspective of Risk Assessment
   * Effect - identify by effects of a risk
   * Cause - identify by cause of a risk
   * Liklihood - assign probability of a risk

## Big O

* steps get added
* drop constants
* different inputs get different variables
* drop non-dominant terms

[<-- Back](../README.md)
