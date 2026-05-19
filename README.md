class Base:
    def __init__(self):
        print("Inside class Base default constructor")

class Derived(Base):
    def __init__(self, x):
        super().__init__()
        print("Inside class Derived constructor, value is ", x)

if __name__ == "__main__":
    obj = Derived(100)


# 🧬 Parameterized Constructor with Inheritance in Python

## 📌 Description

This Python program demonstrates:

* **Inheritance**
* **Parameterized constructor**
* **Constructor chaining using `super()`**

When an object of class `Derived` is created, the constructor of the parent class `Base` is executed first, followed by the parameterized constructor of `Derived`.

---

## 🚀 Features

* Demonstrates constructor inheritance
* Uses parameterized constructor
* Uses `super()` to call parent constructor
* Shows constructor execution order

---

## 🛠️ How It Works

### 1️⃣ Parent Class – `Base`

Contains default constructor:

```python id="u3m8pl"
def __init__(self):
```

Prints:

```text id="n7q2zx"
Inside class Base default constructor
```

---

### 2️⃣ Child Class – `Derived`

```python id="k4m9qa"
class Derived(Base)
```

👉 Inherits from `Base`

Contains parameterized constructor:

```python id="r1x7mv"
def __init__(self, x):
```

Uses:

```python id="p6m3pt"
super().__init__()
```

to call parent constructor.

Then prints value of `x`.

---

## 💻 Code

```python id="x8q2pl"
class Base:
    def __init__(self):
        print("Inside class Base default constructor")

class Derived(Base):
    def __init__(self, x):
        super().__init__()
        print("Inside class Derived constructor, value is ", x)

if __name__ == "__main__":
    obj = Derived(100)
```

---

## ▶️ Output

```id="m5q9zx"
Inside class Base default constructor
Inside class Derived constructor, value is  100
```

---

## 🧠 Key Concepts

### ✔ Parameterized Constructor

Constructor accepting arguments:

```python id="d2m8qa"
def __init__(self, x)
```

---

### ✔ Constructor Chaining

Execution flow:

```text id="f7q3mv"
Derived(100)
      ↓
Base()
      ↓
Derived()
```

---

### ✔ `super()` Keyword

```python id="t4m1pl"
super().__init__()
```

👉 Calls parent class constructor.

---

## 📚 Concepts Used

* Inheritance
* Parameterized constructor
* Constructor chaining
* `super()` method

---

## ⚠️ Important Note

Without:

```python id="z8q6pt"
super().__init__()
```

the `Base` constructor will NOT execute.

---

## 🎯 Why This is Important

This concept is heavily used in:

* Frameworks
* GUI applications
* Real-world OOP systems
* Class initialization chains

---

## 🔧 Future Improvements

* Pass parameters to parent constructor
* Add multilevel inheritance
* Demonstrate method overriding
* Add instance variables

---

## 📄 License

This project is open-source and free to use.
