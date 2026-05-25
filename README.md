# Happy Numbers 😊

A simple Python project to check whether a number is a **Happy Number** or not.

A **Happy Number** is defined by the following process:

1. Start with any positive integer.
2. Replace the number with the sum of the squares of its digits.
3. Repeat the process until:
   - the number becomes `1` → the number is **happy**
   - or the process enters a loop that never reaches `1` → the number is **not happy**

---

## Project Structure

```text
happy-numbers/
│
├── src/
│   └── main.py
│
├── .gitignore
├── LICENSE
└── README.md
```

---

## Features

- Check if a number is happy
- Efficient loop detection using a `set`
- Includes type hints and detailed docstrings
- Beginner-friendly and clean Python code
- Contains simple test assertions

---

## Example

```python
from src.main import is_happy

print(is_happy(19))  # True
print(is_happy(2))   # False
```

---

## How It Works

Example with `19`:

```text
1² + 9² = 82
8² + 2² = 68
6² + 8² = 100
1² + 0² + 0² = 1
```

Since the process reaches `1`, `19` is a happy number.

---

## Requirements

- Python 3.10+

No external libraries are required.

---

## Run the Project

Clone the repository:

```bash
git clone https://github.com/mohamadamin-kazemi/happy-numbers.git
```

Go to the project directory:

```bash
cd happy-numbers
```

Run the program:

```bash
python src/main.py
```

---

## Function Documentation

```python
is_happy(n: int) -> bool
```

### Parameters

| Name | Type | Description |
|------|------|-------------|
| n | int | Number to check |

### Returns

- `True` → if the number is happy
- `False` → otherwise

---

## Tests

The project includes simple assertions:

```python
assert is_happy(19)
assert not is_happy(2)
assert is_happy(7)
assert is_happy(44)
```

---

## License

This project is licensed under the MIT License.

---

## Author

**Mohamadamin Kazemi**
