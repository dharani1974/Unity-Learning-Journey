# Day 2 - C# and Unity Basics

---

## 📚 Topics Covered

### Why Unity Uses C#

- Unity is built on the **.NET** platform, whose primary programming language is **C#**.
- Java and C# have very similar syntax.
- Unity uses C# not because it is faster, but because it integrates well with the .NET ecosystem.
- C# provides useful features for game development such as:
  - Properties
  - Delegates
  - Events

---

## 🚀 Start()

`Start()` runs **only once** when the GameObject is created or when the game starts.

### Common Uses

- Initial setup
- Initializing variables
- Loading data

```csharp
void Start()
{
    Debug.Log("Game Started");
}
```

---

## 🔄 Update()

`Update()` runs **once every frame**.

### Common Uses

- Reading player input
- Moving characters
- Rotating the camera
- Updating gameplay

```csharp
void Update()
{
    if (health <= 0)
    {
        Debug.Log("Player Died");
    }
}
```

---

## 📌 Basic Data Types

```csharp
int health = 100;
float speed = 5.5f;
bool isDead = false;
string playerName = "V";
```

### Data Types

- **int** → Whole numbers
- **float** → Decimal numbers (`f` suffix required)
- **bool** → `true` or `false`
- **string** → Text

---

## ⚡ Why Unity Uses float Instead of double

Unity prefers **float** because it:

- Uses **32 bits** instead of **64 bits**
- Saves memory
- Improves CPU cache efficiency
- Matches GPU hardware for graphics calculations
- Provides enough precision for most gameplay values

---

## 📝 Homework

### Practice

- [x] Install Unity Hub.
- [x] Revise:
  - Variables
  - int
  - float
  - bool
  - string
  - Debug.Log()
  - if statement
  - Start()
  - Update()

### Questions

Answer these in your own words:

1. Why is `Update()` used instead of putting all code in `Start()`?
2. Why does Unity prefer `float` over `double`?
3. What is the purpose of `Debug.Log()`?

---

## 🎯 Key Takeaways

- Unity uses C# because it integrates well with the .NET ecosystem.
- `Start()` runs once for initialization.
- `Update()` runs every frame and handles continuous gameplay logic.
- Understanding basic data types is essential before writing gameplay scripts.
- `float` is preferred for performance and memory efficiency in games.

---

✅ **Status:** Completed