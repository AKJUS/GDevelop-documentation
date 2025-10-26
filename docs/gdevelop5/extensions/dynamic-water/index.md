# Dynamic Water

<img src="https://resources.gdevelop-app.com/assets/Icons/waves.svg" class="extension-icon"></img>
Easily create a realistic liquid surface simulation.

**Authors and contributors** to this experimental extension: [Alios](https://gd.games/Alios).

!!! warning
    This is an extension made by a community member and it only got through a
    light review by the GDevelop extension team. As such, we can't guarantee it
    meets all the quality standards of fully reviewed extensions.

---

FEATURES


- Fully customizable: by adjusting the liquid properties (tension, damping, spreading), you can simulate different types of liquids such as: water, jelly, lava, etc.
- Can obtain the height of the surface at any point
- Allows you to have full control over visual properties such as: color opacity, effects, etc.
- Can create a force at any point on the surface.
- Works on all platforms.


!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.



## Dynamic Water Body 

Easily create a realistic liquid surface simulation. 

### Behavior actions

**Force application**  
Apply a force when an object collides with its surface.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Apply force
    - Parameter 3 (👾 Object): Surface collision of the fluid

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::AddForce`.

**Auto Wave**  
Enable automatic waves.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (❓ Yes or No): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetAutoWave`.

**Show Columns**  
Show the different Column .

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (❓ Yes or No): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetColumn`.

**Springs Number**  
The number of springs controls the distance between the joints and the number of springs. (between 0 and the object width).  
PS: Change the quality of the waves, the more columns the more they use the performance.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetColumnNumber`.

**Damping(d)**  
The spring dampenig value. (between 0 and 0.1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetDamping`.

**Change Period**  
Change Period.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetPeriod`.

**Spread**  
The Spread value will dictate how much a wave oscillation will pass pnto their neighboors.(Between 0 and 0.1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetSpread`.

**Surface Size**  
Change the size of the surface edge.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetSurfaceSize`.

**Tension(k)**  
Greater values will pull the water with greater force. (between 0 and 0.1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetTension`.

**Wave horizontal direction**  
Change the direction of the waves.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔤 String): The water spring constant (one of: "Right", "Left")

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetWaveDirection`.

**Wave Length**  
Change the length of the waves.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetWaveLength`.

**Wave magnitude**  
Change the wave magnitude.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): The water spring constant

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::SetWaveMagnitude`.

**Components**  
Component additions (Visual and Surface Collision).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (👾 Object): Body display
    - Parameter 3 (👾 Object): Object that will be used to detect the collision on the surface

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::WaterBodyAndCollision`.

### Behavior conditions

**Surface collision**  
Test the collision between the object and the fluid surface.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (👾 Object): Define the (physical) object that can interact with the fluid
    - Parameter 3 (👾 Object): Surface collision of the fluid

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `DynamicWater::DynamicWaterBody::CheckSurfaceCollisions`.

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.DynamicWaterBody::ColumnNumber()` | Number of columns. ||
| `Object.DynamicWaterBody::Damping()` | Damping. ||
| `Object.DynamicWaterBody::Spread()` | Spread. ||
| `Object.DynamicWaterBody::SurfaceSize()` | Size of the edge of the surface. ||
| `Object.DynamicWaterBody::Tension()` | Tension. ||


---

*This page is an auto-generated reference page about the **Dynamic Water** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).