# Marching Squares (experimental)

<img src="https://resources.gdevelop-app.com/assets/Icons/peanut-outline.svg" class="extension-icon"></img>
Allow to build a "scalar field" and draw contour lines of it: useful for fog of wars, liquid effects, paint the ground, etc...

**Authors and contributors** to this experimental extension: [D8H](https://gd.games/D8H).

---

It can be helpful for:

  * Liquid effects like water, blobs or lava ([open the project online](https://editor.gdevelop.io/?project=example://marching-squares-liquids))
  * Fog of wars ([open the project online](https://editor.gdevelop.io/?project=example://marching-squares-fog-of-war))
  * Platformer with destructible platforms ([open the project online](https://editor.gdevelop.io/?project=example://marching-squares-platforms-painter))
  * Dynamically paint territories ([open the project online](https://editor.gdevelop.io/?project=example://marching-squares-qix))
  * Top-down relief with physics ([open the project online](https://editor.gdevelop.io/?project=example://marching-squares-terraforming))
  * Island generator ([open the project online](https://editor.gdevelop.io/?project=example://marching-squares-island-generator))

[Read more...](/gdevelop5/extensions/marching-squares/details)

!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.



## Marching squares painter 

Add to a Shape painter object and use the actions to draw a field. Useful for fog of wars, liquid effects (water, lava, blobs...). 

### Behavior actions

**Add a disk**
Add a disk to the field.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Center X
    - Parameter 3 (🔢 Number): Center Y
    - Parameter 4 (🔢 Number): Radius
      The spike height is 1 at this radius.
    - Parameter 5 (🔢 Number): Capping radius ratio
      Small values allow quicker process, but can result to tearing. Try values around 8.
    - Parameter 6 (🔤 String): Operation (one of: "Maximum", "Addition", "Subtraction")

    > Technical note: parameter 7 are internal parameters handled by GDevelop.

**Add a hill**
Add a hill to the field.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Center X
    - Parameter 3 (🔢 Number): Center Y
    - Parameter 4 (🔢 Number): Height
      The hill height at the center, a value of 1 or less means a flat hill.
    - Parameter 5 (🔢 Number): Radius
      The hill height is 1 at this radius.
    - Parameter 6 (🔢 Number): Opacity
      Set to 1 to apply the hill instantly or repeat this action with a lower value to make is progressive.
    - Parameter 7 (🔢 Number): Capping radius ratio
      Small values allow quicker process, but can result to tearing. Try values around 8.
    - Parameter 8 (🔤 String): Operation (one of: "Maximum", "Addition", "Subtraction")

    > Technical note: parameter 9 are internal parameters handled by GDevelop.

**Add a line**
Add a line to the field.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): X position of the start
    - Parameter 3 (🔢 Number): Y position of the start
    - Parameter 4 (🔢 Number): X position of the end
    - Parameter 5 (🔢 Number): Y position of the end
    - Parameter 6 (🔢 Number): Thickness
    - Parameter 7 (🔢 Number): Capping radius ratio
      Small values allow quicker process, but can result to tearing. Try values around 8.
    - Parameter 8 (🔤 String): Operation (one of: "Maximum", "Addition", "Subtraction")

    > Technical note: parameter 9 are internal parameters handled by GDevelop.

**Clamp the field**
Cap every value of the field to a range.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Minimum
    - Parameter 3 (🔢 Number): Maximum

    > Technical note: parameter 4 are internal parameters handled by GDevelop.

**Clear the field**
Clear the field by setting every values to 0.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Draw the contours**
Draw the field contours.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Fill area**
Fill an area of the field from a given location until a given height is reached.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Origin X
    - Parameter 3 (🔢 Number): Origin Y
    - Parameter 4 (🔢 Number): Maximum height
    - Parameter 5 (🔢 Number): Contour thickness
    - Parameter 6 (🔢 Number): Capping radius ratio
      Small values allow quicker process, but can result to tearing. Try values around 8.

    > Technical note: parameter 7 are internal parameters handled by GDevelop.

**Mask a disk**
Mask a disk to the field.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Center X
    - Parameter 3 (🔢 Number): Center Y
    - Parameter 4 (🔢 Number): Radius
      The spike height is 1 at this radius.
    - Parameter 5 (🔢 Number): Capping radius ratio
      Small values allow quicker process, but can result to tearing. Try values around 8.

    > Technical note: parameter 6 are internal parameters handled by GDevelop.

**Mask a line**
Mask a line to the field.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): X position of the start
    - Parameter 3 (🔢 Number): Y position of the start
    - Parameter 4 (🔢 Number): X position of the end
    - Parameter 5 (🔢 Number): Y position of the end
    - Parameter 6 (🔢 Number): Thickness
      The spike height is 1 at this radius.
    - Parameter 7 (🔢 Number): Capping radius ratio
      Small values allow quicker process, but can result to tearing. Try values around 8.

    > Technical note: parameter 8 are internal parameters handled by GDevelop.

**Merge a field**
Apply a given operation on every value of the field using the value from the other field at the same position.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (👾 Object): Field object
    - Parameter 3 (🧩 Behavior): Field behavior
    - Parameter 4 (🔤 String): Operation (one of: "Maximum", "Addition", "Subtraction", "Minimum", "Multiplication", "Division")

    > Technical note: parameter 5 are internal parameters handled by GDevelop.

**Area bounds**
Change the field area bounds.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Left bound
    - Parameter 3 (🔢 Number): Top bound
    - Parameter 4 (🔢 Number): Right bound
    - Parameter 5 (🔢 Number): Bottom bound

    > Technical note: parameter 6 are internal parameters handled by GDevelop.

**Height of the cells**
Change the height of the field cells.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Width of the cells**
Change the width of the field cells.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Fill outside**
Fill outside or inside of the contours.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (❓ Yes or No): Fill outside?

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Grid value**
Change the field value at a grid point.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): X grid index
    - Parameter 3 (🔢 Number): Y grid index
    - Parameter 4 (🔢 Number): Field value

    > Technical note: parameter 5 are internal parameters handled by GDevelop.

**Contour threshold**
Change the contour threshold.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 are internal parameters handled by GDevelop.

**Transform the field**
Apply an affine on the field values.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Coefficient
    - Parameter 3 (🔢 Number): Offset

    > Technical note: parameter 4 are internal parameters handled by GDevelop.

**Update hitboxes**
Update the field hitboxes.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Unfill area**
Unfill an area of the field from a given location until a given height is reached.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Origin X
    - Parameter 3 (🔢 Number): Origin Y
    - Parameter 4 (🔢 Number): Minimum height
    - Parameter 5 (🔢 Number): Contour thickness
    - Parameter 6 (🔢 Number): Capping radius ratio
      Small values allow quicker process, but can result to tearing. Try values around 8.

    > Technical note: parameter 7 are internal parameters handled by GDevelop.

### Behavior conditions

**Field value**
Check if a field is greater than a given value.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): X position of the point
    - Parameter 3 (🔢 Number): Y position of the point
    - Parameter 4 (🔢 Number): Value

    > Technical note: parameter 5 are internal parameters handled by GDevelop.

**Fill outside**
Check if the contours are filled outside.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 are internal parameters handled by GDevelop.

**Point is inside**
Check if a point is inside the contour.

??? quote "See parameters"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): X position of the point
    - Parameter 3 (🔢 Number): Y position of the point

    > Technical note: parameter 4 are internal parameters handled by GDevelop.

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.MarchingSquaresBehavior::AreaBottom()` | Area bottom bound of the field. ||
| `Object.MarchingSquaresBehavior::AreaLeft()` | Area left bound of the field. ||
| `Object.MarchingSquaresBehavior::AreaRight()` | Area right bound of the field. ||
| `Object.MarchingSquaresBehavior::AreaTop()` | Area top bound of the field. ||
| `Object.MarchingSquaresBehavior::CellHeight()` | Height of the field cells. ||
| `Object.MarchingSquaresBehavior::CellWidth()` | Width of the field cells. ||
| `Object.MarchingSquaresBehavior::ContourThreshold()` | The contour threshold. ||
| `Object.MarchingSquaresBehavior::DimensionX()` | The number of cells on the x axis. ||
| `Object.MarchingSquaresBehavior::DimensionY()` | The number of cells on the y axis. ||
| `Object.MarchingSquaresBehavior::FieldValue(number, number)` | The field value at a given location. ||
| | _🔢 Number_ | X position of the point |
| | _🔢 Number_ | Y position of the point |
| `Object.MarchingSquaresBehavior::GridValue(number, number)` | The field value at a grid point. ||
| | _🔢 Number_ | X grid index |
| | _🔢 Number_ | Y grid index |
| `Object.MarchingSquaresBehavior::NormalX(number, number)` | The normal X coordinate at a given location. ||
| | _🔢 Number_ | X position of the point |
| | _🔢 Number_ | Y position of the point |
| `Object.MarchingSquaresBehavior::NormalY(number, number)` | The normal Y coordinate at a given location. ||
| | _🔢 Number_ | X position of the point |
| | _🔢 Number_ | Y position of the point |
| `Object.MarchingSquaresBehavior::NormalZ(number, number)` | The normal Z coordinate at a given location. ||
| | _🔢 Number_ | X position of the point |
| | _🔢 Number_ | Y position of the point |


---

*This page is an auto-generated reference page about the **Marching Squares (experimental)** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).