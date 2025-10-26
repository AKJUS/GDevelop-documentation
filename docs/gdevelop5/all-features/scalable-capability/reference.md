# Scalable objects Reference

Actions/conditions/expression to change or check the scale of an object (default: 1). [Read more explanations about it.](/gdevelop5/objects)



## Scalable objects 

Actions/conditions/expression to change or check the scale of an object (default: 1). 

### Behavior actions

**Scale**  
Change the scale of the object (default scale is 1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Scale (1 by default)

    > Technical note: this action internal type (in GDevelop JSON) is `ScalableCapability::ScalableBehavior::SetValue`.

**Scale on X axis**  
Change the scale on X axis of the object (default scale is 1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Scale (1 by default)

    > Technical note: this action internal type (in GDevelop JSON) is `ScalableCapability::ScalableBehavior::SetX`.

**Scale on Y axis**  
Change the scale on Y axis of the object (default scale is 1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Scale (1 by default)

    > Technical note: this action internal type (in GDevelop JSON) is `ScalableCapability::ScalableBehavior::SetY`.

### Behavior conditions

**Scale**  
Compare the scale of the object (default scale is 1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Scale (1 by default)

    > Technical note: this condition internal type (in GDevelop JSON) is `ScalableCapability::ScalableBehavior::Value`.

**Scale on X axis**  
Compare the scale on X axis of the object (default scale is 1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Scale (1 by default)

    > Technical note: this condition internal type (in GDevelop JSON) is `ScalableCapability::ScalableBehavior::X`.

**Scale on Y axis**  
Compare the scale on Y axis of the object (default scale is 1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Scale (1 by default)

    > Technical note: this condition internal type (in GDevelop JSON) is `ScalableCapability::ScalableBehavior::Y`.

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.Scale::Value()` | Return the scale of the object (default scale is 1). ||
| `Object.Scale::X()` | Return the scale on X axis of the object (default scale is 1). ||
| `Object.Scale::Y()` | Return the scale on Y axis of the object (default scale is 1). ||



---

The Scalable objects extension is always installed in all GDevelop projects: there is no need to add it from the Project Manager.

*This page is an auto-generated reference page about the **Scalable objects** feature of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop features here](/gdevelop5/all-features).