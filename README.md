[![Work in Repl.it](https://classroom.github.com/assets/work-in-replit-14baed9a392b3a25080506f3b7b6d57f295ec2978f6f33ec97e36a161684cbe9.svg)](https://classroom.github.com/online_ide?assignment_repo_id=4490527&assignment_repo_type=AssignmentRepo)
# Exercise 5.10 Comparing apartments

In the estate agent's information system, an apartment that is on sale is represented by an object that is instantiated from the following class:

```python
class Apartment:

    def __init__(self, rooms, squares, price_per_square):
        self.rooms = rooms
        self.square = squares
        self.price_per_square = price_per_square
```

Your task is to create a few methods that can be used to compare apartments that are being sold.

## Comparing sizes

Create a method `larger_than(self, other)` that returns true if the apartment object whose method is called has a larger total area than the apartment object that is being compared.

An example of how the method should work:

```python
manhattan_studio_apt = Apartment(1, 16, 5500)
atlanta_two_bedroom_apt = Apartment(2, 38, 4200)
bangor_three_bedroom_apt = Apartment(3, 78, 2500)

print(manhattan_studio_apt.larger_than(atlanta_two_bedroom_apt)) # false
print(bangor_three_bedroom_apt.larger_than(atlanta_two_bedroom_apt)) # true
```

## Price difference

Create a method `price_difference(self, other)` that returns the price difference of the apartment object whose method was called and the apartment object received as the parameter. The price difference is the absolute value of the difference of the prices (price can be calculated by multiplying the price per square by the number of squares).

An example of how the method should work:

```python
manhattan_studio_apt = Apartment(1, 16, 5500)
atlanta_two_bedroom_apt = Apartment(2, 38, 4200)
bangor_three_bedroom_apt = Apartment(3, 78, 2500)

print(manhattan_studio_apt.price_difference(atlanta_two_bedroom_apt))  # 71600
print(bangor_three_bedroom_apt.price_difference(atlanta_two_bedroom_apt))   # 35400
```

## More expensive?

Write a method `more_expensive_than(self,other)` that returns true if the apartment object whose method is called is more expensive than the apartment object being compared.

An example of how the method should work:

```python
manhattan_studio_apt = Apartment(1, 16, 5500)
atlanta_two_bedroom_apt = Apartment(2, 38, 4200)
bangor_three_bedroom_apt = Apartment(3, 78, 2500)

print(manhattan_studio_apt.more_expensive_than(atlanta_two_bedroom_apt))  # true
print(bangor_three_bedroom_apt.more_expensive_than(atlanta_two_bedroom_apt))   # false
```
