# Conversion Reference

Expressions to convert numbers to string, strings to numbers, angles (degrees from/to radians) and a GDevelop variable to/from a JSON string. [Read more explanations about it.](/gdevelop5/all-features/common-conversions)

## Actions

**Convert JSON to object variable**
Parse a JSON object and store it into an object variable

??? quote "See parameters"

    - Parameter 0 (string): JSON string
    - Parameter 1: 👾 Object
    - Parameter 2 (🗄️ Object variable): Object variable where store the JSON object

**Convert JSON to a variable**
Parse a JSON object and store it into a variable

??? quote "See parameters"

    - Parameter 0 (string): JSON string
    - Parameter 1 (🗄️ Any variable): Variable where to store the JSON object

## Expressions

| Expression | Description |  |
|-----|-----|-----|
| `LargeNumberToString(number)` | Convert the result of the expression to text, without using the scientific notation ||
| | _🔢 Number_ | Expression to be converted to text |
| `ObjectVarToJSON(object, object variable)` | Convert an object variable to JSON ||
| | _👾 Object_ | The object with the variable |
| | _🗄️ Object variable_ | The object variable to be stringified |
| `ToDeg(number)` | Converts the angle, expressed in radians, into degrees ||
| | _🔢 Number_ | Angle, in radians |
| `ToJSON(variable)` | Convert a variable to JSON ||
| | _🗄️ Any variable_ | The variable to be stringified |
| `ToNumber(string)` | Convert the text to a number ||
| | _string_ | Text to convert to a number |
| `ToRad(number)` | Converts the angle, expressed in degrees, into radians ||
| | _🔢 Number_ | Angle, in degrees |
| `ToString(number)` | Convert the result of the expression to text ||
| | _🔢 Number_ | Expression to be converted to text |



---

The Conversion extension is always installed in all GDevelop projects: there is no need to add it from the Project Manager.

*This page is an auto-generated reference page about the **Conversion** feature of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop features here](/gdevelop5/all-features).