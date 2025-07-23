# 🔐 Random Password Generator

A simple and secure password generator written in Python that creates strong, randomized passwords using letters, numbers, and special characters.

## 💡 Features

- Generates secure, random passwords
- Customizable password length
- Uses Python's built-in `random` and `string` libraries
- Easy to read, simple to extend

## 🧪 How It Works

The script combines ASCII letters (uppercase and lowercase), digits, and punctuation to form a pool of characters. It then randomly selects characters from this pool to build a password of the desired length.

## 🛠️ Code

```python
import random
import string

def generate_random_password(length=12):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

random_password = generate_random_password()
print("Random Password:", random_password)
