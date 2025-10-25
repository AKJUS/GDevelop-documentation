# Multitouch joystick and buttons (sprite)

<img src="https://resources.gdevelop-app.com/assets/Icons/Line Hero Pack/Master/SVG/Videogames/Videogames_controller_joystick_arrows_direction.svg" class="extension-icon"></img>
Joysticks or buttons for touchscreens.

**Authors and contributors** to this experimental extension: [VictrisGames](https://gd.games/VictrisGames), [MelonDev](https://gd.games/MelonDev), [xellix](https://gd.games/xellix), [D8H](https://gd.games/D8H).

---

Multitouch joysticks are objects showing a joystick on the screen, useful for mobile. They work like a physical gamepad:

- 4 or 8 directions
- Analogus pads
- Player selection
- Automatic "mapper" behaviors for 2D and 3D movement behaviors (platformer characters, top-down movement, 3D character etc...). Add one of these to the object with the movement behavior (i.e: the player most of the time) and the behavior will then be controlled automatically by the virtual joystick (it works by reading the multitouch joystick state and simulating controls). No need for additional events to make it work once the behaviors are set up.

There are ready-to-use joysticks in the asset-store [multitouch joysticks pack](https://editor.gdevelop.io/?initial-dialog=asset-store&asset-pack=multitouch-joysticks-multitouch-joysticks).

[Read more...](/gdevelop5/objects/multitouch-joystick)

!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.

## Conditions

**New touch on a screen side**  
Check if a new touch has started on the right or left side of the screen.

??? quote "See parameters & details"

    - Parameter 1 (👾 Object): Multitouch joystick
    - Parameter 2 (🔤 String): Screen side (one of: "Left", "Right")

    > Technical note: parameters 0, 3 are internal parameters handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::HasTouchStartedOnScreenSide`.

**Multitouch controller button just pressed**  
Check if a button was just pressed on a multitouch controller.

??? quote "See parameters & details"

    - Parameter 1 (🔢 Number): Multitouch controller identifier (1, 2, 3, 4...)
    - Parameter 2 (string): Button name

    > Technical note: parameters 0, 3 are internal parameters handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::IsButtonJustPressed`.

**Multitouch controller button pressed**  
Check if a button is pressed on a multitouch controller.

??? quote "See parameters & details"

    - Parameter 1 (🔢 Number): Multitouch controller identifier (1, 2, 3, 4...)
    - Parameter 2 (string): Button name

    > Technical note: parameters 0, 3 are internal parameters handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::IsButtonPressed`.

**Multitouch controller button released**  
Check if a button is released on a multitouch controller.

??? quote "See parameters & details"

    - Parameter 1 (🔢 Number): Multitouch controller identifier (1, 2, 3, 4...)
    - Parameter 2 (string): Button name

    > Technical note: parameters 0, 3 are internal parameters handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::IsButtonReleased`.

**Joystick pushed in a direction (4-way)**  
Check if joystick is pushed in a given direction.

??? quote "See parameters & details"

    - Parameter 1 (🔢 Number): Multitouch controller identifier (1, 2, 3, 4...)
    - Parameter 2 (🔤 String): Joystick name (one of: "Primary", "Secondary")
    - Parameter 3 (🔤 String): Direction (one of: "Up", "Down", "Left", "Right")

    > Technical note: parameters 0, 4 are internal parameters handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::IsDirectionPushed4Way`.

**Joystick pushed in a direction (8-way)**  
Check if joystick is pushed in a given direction.

??? quote "See parameters & details"

    - Parameter 1 (🔢 Number): Multitouch controller identifier (1, 2, 3, 4...)
    - Parameter 2 (🔤 String): Joystick name (one of: "Primary", "Secondary")
    - Parameter 3 (🔤 String): Direction (one of: "Up", "Down", "Left", "Right", "UpLeft", "UpRight", "DownLeft", "DownRight")

    > Technical note: parameters 0, 4 are internal parameters handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::IsDirectionPushed8Way`.

**Stick force**  
Compare the force of multitouch contoller stick (from 0 to 1).

??? quote "See parameters & details"

    - Parameter 1: 🟰 Relational operator
    - Parameter 2 (🔢 Number): Value to compare
    - Parameter 3 (🔢 Number): Multitouch controller identifier (1, 2, 3, 4...)
    - Parameter 4 (🔤 String): Stick name (one of: "Primary", "Secondary")

    > Technical note: parameters 0, 5 are internal parameters handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::StickForce`.

## Expressions

| Expression | Description |  |
|-----|-----|-----|
| `SpriteMultitouchJoystick::StickAngle(number, string)` | Return the angle the multitouch controller stick is pointing towards (Range: -180 to 180). ||
| | _🔢 Number_ | Multitouch controller identifier (1, 2, 3, 4...) |
| | _🔤 String_ | Joystick name |
| `SpriteMultitouchJoystick::StickForce(number, string)` | Return the force of multitouch contoller stick (from 0 to 1). ||
| | _🔢 Number_ | Multitouch controller identifier (1, 2, 3, 4...) |
| | _🔤 String_ | Stick name |
| `SpriteMultitouchJoystick::StickForceX(number, string)` | Return the multitouch contoller stick force on X axis (from -1 at the left to 1 at the right). ||
| | _🔢 Number_ | Multitouch controller identifier (1, 2, 3, 4...) |
| | _🔤 String_ | Joystick name |
| `SpriteMultitouchJoystick::StickForceY(number, string)` | Return the multitouch contoller stick force on Y axis (from -1 at the top to 1 at the bottom). ||
| | _🔢 Number_ | Multitouch controller identifier (1, 2, 3, 4...) |
| | _🔤 String_ | Joystick name |

## Multitouch Joystick 

Joystick for touchscreens. 

### Object actions

**De/activate control**  
De/activate control of the joystick.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1 (❓ Yes or No): Activate

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::ActivateControl`.

**Multitouch controller identifier**  
Change the multitouch controller identifier (1, 2, 3, 4...).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Operator
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::SetControllerIdentifier`.

**Dead zone radius**  
Change the dead zone radius of the joystick (range: 0 to 1). The deadzone is an area for which movement on sticks won't be taken into account (instead, the stick will be considered as not moved).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Operator
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::SetDeadZoneRadius`.

**Joystick name**  
Change the joystick name of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Operator
    - Parameter 2 (string): Value

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::SetJoystickIdentifier`.

**Show and start pressing**  
Show the joystick until it is released.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object

    > Technical note: parameter 1 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::TeleportAndPress`.

### Object conditions

**Multitouch controller identifier**  
Compare the multitouch controller identifier (1, 2, 3, 4...).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Relational operator
    - Parameter 2 (🔢 Number): Value to compare

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::ControllerIdentifier`.

**Dead zone radius**  
Compare the dead zone radius of the joystick (range: 0 to 1). The deadzone is an area for which movement on sticks won't be taken into account (instead, the stick will be considered as not moved).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Relational operator
    - Parameter 2 (🔢 Number): Value to compare

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::DeadZoneRadius`.

**Joystick pushed in a direction (4-way movement)**  
Check if joystick is pushed in a given direction.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1 (🔤 String): Direction (one of: "Up", "Down", "Left", "Right")

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::IsDirectionPushed4Way`.

**Joystick pushed in a direction (8-way movement)**  
Check if joystick is pushed in a given direction.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1 (🔤 String): Direction (one of: "Up", "Down", "Left", "Right", "UpLeft", "UpRight", "DownLeft", "DownRight")

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::IsDirectionPushed8Way`.

**Stick pressed**  
Check if a stick is pressed.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object

    > Technical note: parameter 1 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::IsPressed`.

**Joystick name**  
Compare the joystick name of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Relational operator
    - Parameter 2 (string): Value to compare

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::JoystickIdentifier`.

**Stick force**  
Compare the strick force (from 0 to 1).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Relational operator
    - Parameter 2 (🔢 Number): Value to compare

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::StickForce`.

**Stick X force**  
Compare the stick force on X axis (from -1 at the left to 1 at the right).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Relational operator
    - Parameter 2 (🔢 Number): Value to compare

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::StickForceX`.

**Stick Y force**  
Compare the stick force on Y axis (from -1 at the top to 1 at the bottom).

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Relational operator
    - Parameter 2 (🔢 Number): Value to compare

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::SpriteMultitouchJoystick::StickForceY`.

### Object expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.ControllerIdentifier()` | Return the multitouch controller identifier (1, 2, 3, 4...). ||
| `Object.DeadZoneRadius()` | Return the dead zone radius of the joystick (range: 0 to 1). The deadzone is an area for which movement on sticks won't be taken into account (instead, the stick will be considered as not moved). ||
| `Object.JoystickIdentifier()` | Return the joystick name of the object. ||
| `Object.StickAngle()` | Return the angle the stick is pointing towards (from -180 to 180). ||
| `Object.StickForce()` | Return the strick force (from 0 to 1). ||
| `Object.StickForceX()` | Return the stick force on X axis (from -1 at the left to 1 at the right). ||
| `Object.StickForceY()` | Return the stick force on Y axis (from -1 at the top to 1 at the bottom). ||

## First person camera multitouch controller mapper 

Control camera rotations with a multitouch controller. 

### Behavior actions

**Horizontal rotation acceleration**  
Change the horizontal rotation acceleration of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::SetHorizontalRotationAcceleration`.

**Horizontal rotation deceleration**  
Change the horizontal rotation deceleration of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::SetHorizontalRotationDeceleration`.

**Maximum horizontal rotation speed**  
Change the maximum horizontal rotation speed of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::SetHorizontalRotationSpeedMax`.

**Z position offset**  
Change the z position offset of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::SetOffsetZ`.

**Maximum vertical camera angle**  
Change the maximum vertical camera angle of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::SetVerticalAngleMax`.

**Minimum vertical camera angle**  
Change the minimum vertical camera angle of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::SetVerticalAngleMin`.

**Vertical rotation acceleration**  
Change the vertical rotation acceleration of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::SetVerticalRotationAcceleration`.

**Vertical rotation deceleration**  
Change the vertical rotation deceleration of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::SetVerticalRotationDeceleration`.

**Maximum vertical rotation speed**  
Change the maximum vertical rotation speed of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Operator
    - Parameter 3 (🔢 Number): Value

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::SetVerticalRotationSpeedMax`.

### Behavior conditions

**Horizontal rotation acceleration**  
Compare the horizontal rotation acceleration of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::HorizontalRotationAcceleration`.

**Horizontal rotation deceleration**  
Compare the horizontal rotation deceleration of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::HorizontalRotationDeceleration`.

**Maximum horizontal rotation speed**  
Compare the maximum horizontal rotation speed of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::HorizontalRotationSpeedMax`.

**Z position offset**  
Compare the z position offset of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::OffsetZ`.

**Maximum vertical camera angle**  
Compare the maximum vertical camera angle of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::VerticalAngleMax`.

**Minimum vertical camera angle**  
Compare the minimum vertical camera angle of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::VerticalAngleMin`.

**Vertical rotation acceleration**  
Compare the vertical rotation acceleration of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::VerticalRotationAcceleration`.

**Vertical rotation deceleration**  
Compare the vertical rotation deceleration of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::VerticalRotationDeceleration`.

**Maximum vertical rotation speed**  
Compare the maximum vertical rotation speed of the object.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2: 🟰 Relational operator
    - Parameter 3 (🔢 Number): Value to compare

    > Technical note: parameter 4 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::FirstPersonMultitouchMapper::VerticalRotationSpeedMax`.

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.FirstPersonMultitouchMapper::HorizontalRotationAcceleration()` | Return the horizontal rotation acceleration of the object. ||
| `Object.FirstPersonMultitouchMapper::HorizontalRotationDeceleration()` | Return the horizontal rotation deceleration of the object. ||
| `Object.FirstPersonMultitouchMapper::HorizontalRotationSpeedMax()` | Return the maximum horizontal rotation speed of the object. ||
| `Object.FirstPersonMultitouchMapper::OffsetZ()` | Return the z position offset of the object. ||
| `Object.FirstPersonMultitouchMapper::VerticalAngleMax()` | Return the maximum vertical camera angle of the object. ||
| `Object.FirstPersonMultitouchMapper::VerticalAngleMin()` | Return the minimum vertical camera angle of the object. ||
| `Object.FirstPersonMultitouchMapper::VerticalRotationAcceleration()` | Return the vertical rotation acceleration of the object. ||
| `Object.FirstPersonMultitouchMapper::VerticalRotationDeceleration()` | Return the vertical rotation deceleration of the object. ||
| `Object.FirstPersonMultitouchMapper::VerticalRotationSpeedMax()` | Return the maximum vertical rotation speed of the object. ||

## Multitouch button 

Detect presses made on a touchscreen on the object so it acts like a button and automatically trigger the button having the same identifier for the mapper behaviors. 

### Behavior conditions

**Button just pressed**  
Check if the button was just pressed.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::MultitouchButton::IsJustPressed`.

**Button pressed**  
Check if the button is pressed.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::MultitouchButton::IsPressed`.

**Button released**  
Check if the button is released.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `SpriteMultitouchJoystick::MultitouchButton::IsReleased`.

_No expressions for this behavior._


## 3D car multitouch controller mapper 

Control a 3D physics car with a multitouch controller. 

_No expressions for this behavior._


## 3D platformer multitouch controller mapper 

Control a 3D physics character with a multitouch controller. 

_No expressions for this behavior._


## Platformer multitouch controller mapper 

Control a platformer character with a multitouch controller. 

_No expressions for this behavior._


## 3D shooter multitouch controller mapper 

Control a 3D physics character with a multitouch controller. 

_No expressions for this behavior._


## Top-down multitouch controller mapper 

Control a top-down character with a multitouch controller. 

_No expressions for this behavior._



---

*This page is an auto-generated reference page about the **Multitouch joystick and buttons (sprite)** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).