# Python `random` Module Cheat Sheet

## 1. **Importing the Random Module**
```python
import random
```

## 2. **Generating Random Numbers**
```python
print(random.random())  # Random float between 0 and 1
print(random.uniform(10, 20))  # Random float between 10 and 20
print(random.randint(1, 10))  # Random integer between 1 and 10 (inclusive)
print(random.randrange(1, 10, 2))  # Random odd number from 1 to 9
```

## 3. **Random Choice from a List**
```python
my_list = ['apple', 'banana', 'cherry']
print(random.choice(my_list))  # Randomly selects one item
print(random.choices(my_list, k=2))  # Randomly selects 2 items (with replacement)
print(random.sample(my_list, 2))  # Randomly selects 2 items (without replacement)
```

## 4. **Shuffling a List**
```python
random.shuffle(my_list)  # Shuffles the list in place
print(my_list)
```

## 5. **Random Boolean Values**
```python
print(random.choice([True, False]))  # Randomly selects True or False
```

## 6. **Seeding for Reproducibility**
```python
random.seed(42)  # Sets seed for reproducibility
print(random.random())  # Generates the same random number each time
```

## 7. **Generating Random Gaussian Distribution**
```python
print(random.gauss(mu=0, sigma=1))  # Random number from a Gaussian distribution
```

---
This cheat sheet covers essential Python `random` module functions. 🚀
