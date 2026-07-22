# Day 4 - GameObjects and Components

---

# GameObject

A **GameObject** is any object that exists in a Unity scene.

Examples:

- Player
- Enemy
- Tree
- Car
- House
- Ball

A GameObject by itself is just an empty object. It becomes useful only after adding components.

---

# Components

Components give a GameObject its functionality.

Example:

```text
Player (GameObject)

├── Transform
├── Mesh Renderer
├── Rigidbody
├── Capsule Collider
└── Player Script
```

Each component has a specific purpose.

---

# Transform

Every GameObject automatically has a **Transform** component.

It stores:

- Position
- Rotation
- Scale

Without a Transform, Unity would not know where an object is, how it is rotated, or how large it should be.

---

# Rigidbody

A Rigidbody allows Unity's physics engine to control the object.

With a Rigidbody:

- Gravity works
- Objects can fall
- Forces can be applied
- Objects can collide naturally

Without a Rigidbody:

- No gravity
- No falling
- No physics-based movement

---

# Collider

A Collider defines the physical boundary of an object.

Common types:

- Box Collider
- Sphere Collider
- Capsule Collider

A Collider allows Unity to detect collisions.

Without a Collider, other objects can pass straight through the object.

---

# Mesh Renderer

The Mesh Renderer makes a 3D model visible in the game.

Without a Mesh Renderer:

- The object still exists.
- The object can still have physics and scripts.
- It becomes invisible in the Scene and Game view.

---

# Script

Scripts contain the C# code that controls the GameObject's behavior.

Examples:

- Player movement
- Enemy AI
- Opening doors
- Collecting coins

---

# Hierarchy

The Hierarchy window displays every GameObject in the current scene.

It also shows the relationship between objects.

---

# Parent and Child

Example:

```text
Player
│
├── Head
├── Left Hand
├── Right Hand
└── Gun
```

If the Player moves:

- Head moves
- Hands move
- Gun moves

All child objects follow their parent automatically.

This relationship is used throughout Unity to organize objects.

---

# My Understanding

- Every object in a game is a **GameObject**.
- A GameObject is empty until Components are added.
- Every GameObject has a Transform because every object needs a position, rotation, and scale.
- Rigidbody adds physics like gravity and falling.
- Collider defines the object's physical boundary and prevents objects from passing through.
- Mesh Renderer makes the object visible.
- Scripts control how a GameObject behaves.
- Parent and Child relationships help multiple objects move together.

---

# Summary

- GameObject = Object
- Component = Functionality
- Transform = Position, Rotation, Scale
- Rigidbody = Physics
- Collider = Collision
- Mesh Renderer = Visibility
- Script = Behaviour
- Hierarchy = Organizes GameObjects

---

✅ **Status:** Completed