# Day 3 - Unity Input System and Operators

---

# Unity Input Functions

## Input.GetKey()

- Returns `true` as long as the key is being held down.
- The code executes every frame while the key is pressed.
- Used for continuous actions.

### Example

```csharp
if (Input.GetKey(KeyCode.W))
{
    Debug.Log("Moving Forward");
}
```

If **W** is held for **3 seconds** at **60 FPS**, `Update()` runs about **180 times**, so `"Moving Forward"` is printed about **180 times**.

### Common Uses

- Walking
- Running
- Moving a vehicle
- Camera movement

---

## Input.GetKeyDown()

- Returns `true` only once when the key is first pressed.
- Holding the key does not repeatedly trigger the action.
- Used for one-time actions.

### Example

```csharp
if (Input.GetKeyDown(KeyCode.Space))
{
    Debug.Log("Jump");
}
```

### Common Uses

- Jumping
- Reloading
- Opening doors
- Shooting a single bullet

---

## Input.GetKeyUp()

- Returns `true` once when the key is released.
- Useful for detecting when an action has finished.

### Example

```csharp
if (Input.GetKeyUp(KeyCode.W))
{
    Debug.Log("Stopped Moving");
}
```

### Common Uses

- Stop moving
- Stop charging an attack
- Release an object

---

# Operators

## Arithmetic Operators

Used for mathematical calculations.

```csharp
health = health - 20;
score = score + 100;
coins++;
health += 20;
```

Common operators:

- `+` Addition
- `-` Subtraction
- `*` Multiplication
- `/` Division
- `++` Increment
- `--` Decrement
- `+=` Add and assign
- `-=` Subtract and assign

---

## Comparison Operators

Used to compare two values.

```csharp
health == 100
health != 100
health >= 100
```

Common operators:

- `==` Equal to
- `!=` Not equal to
- `>` Greater than
- `<` Less than
- `>=` Greater than or equal to
- `<=` Less than or equal to

Comparison operators always return either **true** or **false**.

---

## Logical Operators

Used to combine multiple conditions.

### AND (`&&`)

Returns **true** only when both conditions are true.

### OR (`||`)

Returns **true** if at least one condition is true.

### NOT (`!`)

Reverses the result of a boolean value.

---

# Mini Challenge

### Scenario

- Player has **5 bullets**.
- The player presses the left mouse button once.
- Then holds the button for **2 seconds**.
- Shooting uses **Input.GetKeyDown()**.

### Explanation

Only **one shot** is fired because `Input.GetKeyDown()` runs only when the button is initially pressed.

- Shots fired: **1**
- Remaining bullets: **4**

Holding the button does not fire additional shots because `Input.GetKeyDown()` does not execute repeatedly while the button is held.

---

# Summary

- `Input.GetKey()` → Continuous actions.
- `Input.GetKeyDown()` → One-time actions.
- `Input.GetKeyUp()` → Detect key release.
- Arithmetic operators perform calculations.
- Comparison operators compare values.
- Logical operators combine multiple conditions.

---

✅ **Status:** Completed