# 3D physics character animator

<img src="https://resources.gdevelop-app.com/assets/Icons/Glyphster Pack/Master/SVG/Sports and Fitness/Sports and Fitness_training_running_run.svg" class="extension-icon"></img>
Change animations of a 3D physics character automatically.

**Authors and contributors** to this experimental extension: [D8H](https://gd.games/D8H).

---

Automatically change the animationsof a 3D physics character based on movement and interaction with platform objects.

The 3D platformer example uses this extension ([open the project online](https://editor.gdevelop.io/?project=example://3d-platformer)).

!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.



## 3D physics character animator 

Change animations of a 3D physics character automatically. 

### Behavior actions

**Rotation speed**  
Change the rotation speed of the object.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 are internal parameters handled by GDevelop.

### Behavior conditions

**Rotation speed**  
Compare the rotation speed of the object.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 are internal parameters handled by GDevelop.

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.PhysicsCharacter3DAnimator::RotationSpeed()` | Return the rotation speed of the object. ||


---

*This page is an auto-generated reference page about the **3D physics character animator** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).