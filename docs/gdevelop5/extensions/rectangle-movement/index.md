# Rectangular movement

<img src="https://resources.gdevelop-app.com/assets/Icons/shape-rectangle-plus.svg" class="extension-icon"></img>
Move objects in a rectangular pattern.

**Authors and contributors** to this experimental extension: [4ian](https://gd.games/4ian), [VictrisGames](https://gd.games/VictrisGames), [D8H](https://gd.games/D8H).

---

Move objects in a rectangular pattern with easing functions from the Tween extension.

It can be used for:


- Moveable platforms
- Enemy movement patterns
- Moving along the border of another object (inside, center, outside)

The platformer example uses this extension ([open the project online](https://editor.gdevelop.io/?project=example://platformer)).

This game shows how to make objects move around the border of another object ([open the project online](https://editor.gdevelop.io/?project=example://moving-saw-platformer)).

This example can be used to test different settings ([open the project online](https://editor.gdevelop.io/?project=example://rectangular-movement)).


!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.

## Actions

**Update rectangular movement to follow the border of an object**  
Update rectangular movement to follow the border of an object. Run once, or every time the center object moves.

??? quote "See parameters"

    - Parameter 1 (👾 Object): Moving object
    - Parameter 2 (🧩 Behavior): Rectangle Movement (required)
    - Parameter 3 (👾 Object): Center object
    - Parameter 4 (🔤 String): Position on border (one of: "Inside", "Center", "Outside")

    > Technical note: parameters 0, 5 are internal parameters handled by GDevelop.

**Move to the nearest corner of the center object**  
Move to the nearest corner of the center object.

??? quote "See parameters"

    - Parameter 1 (👾 Object): Moving object
    - Parameter 2 (🧩 Behavior): Rectangle Movement (required)
    - Parameter 3 (👾 Object): Center object

    > Technical note: parameters 0, 4 are internal parameters handled by GDevelop.



## Rectangular movement 

Move objects in a rectangular pattern. 

### Behavior actions

**Bottom bound**  
Change the bottom bound of the rectangular movement.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Clockwise**  
Change the direction to clockwise or counter-clockwise.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (❓ Yes or No): Clockwise

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Easing**  
Change the easing function of the movement.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔤 String): Easing (one of: "linear", "easeInQuad", "easeOutQuad", "easeInOutQuad", "easeInCubic", "easeOutCubic", "easeInOutCubic", "easeInQuart", "easeOutQuart", "easeInOutQuart", "easeInQuint", "easeOutQuint", "easeInOutQuint", "easeInOutSine", "easeInExpo", "easeOutExpo", "easeInOutExpo", "easeInCirc", "easeOutCirc", "easeInOutCirc", "easeOutBounce", "easeInBack", "easeOutBack", "easeInOutBack", "elastic", "swingFromTo", "swingFrom", "swingTo", "bounce", "bouncePast", "easeFromTo", "easeFrom", "easeTo")

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Horizontal edge duration**  
Change the time the object takes to go through a horizontal edge (in seconds).

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Left bound**  
Change the left bound of the rectangular movement.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Right bound**  
Change the right bound of the rectangular movement.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Top bound**  
Change the top bound of the rectangular movement.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Vertical edge duration**  
Change the time the object takes to go through a vertical edge (in seconds).

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Teleport at a corner**  
Teleport the object to a corner of the movement rectangle.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔤 String): Corner (one of: "Top-left corner", "Top-right corner", "Bottom-left corner", "Bottom-right corner")

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Toggle direction**  
Toggle the direction to clockwise or counter-clockwise.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

### Behavior conditions

**Is moving clockwise**  
Check if the object is moving clockwise.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Is moving down**  
Check if the object is moving down.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Is moving left**  
Check if the object is moving to the left.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Is moving right**  
Object is moving to the right.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Is moving up**  
Check if the object is moving up.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Is on bottom**  
Object is on the bottom side of the rectangle.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Is on left**  
Object is on the left side of the rectangle.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Is on right**  
Object is on the right side of the rectangle.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Is on top**  
Object is on the top side of the rectangle.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.RectangleMovement::Bottom()` | Return the bottom bound of the movement. ||
| `Object.RectangleMovement::Height()` | Return the rectangle height. ||
| `Object.RectangleMovement::HorizontalEdgeDuration()` | Return the time the object takes to go through a horizontal edge (in seconds). ||
| `Object.RectangleMovement::Left()` | Return the left bound of the movement. ||
| `Object.RectangleMovement::LoopDuration()` | Return the time the object takes to go through the whole rectangle (in seconds). ||
| `Object.RectangleMovement::Perimeter()` | Return the perimeter of the movement rectangle. ||
| `Object.RectangleMovement::Right()` | Return the right bound of the movement. ||
| `Object.RectangleMovement::Top()` | Return the top bound of the movement. ||
| `Object.RectangleMovement::VerticalEdgeDuration()` | Return the time the object takes to go through a vertical edge (in seconds). ||
| `Object.RectangleMovement::Width()` | Return the rectangle width. ||


---

*This page is an auto-generated reference page about the **Rectangular movement** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).