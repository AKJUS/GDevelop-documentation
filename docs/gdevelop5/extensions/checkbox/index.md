# Checkbox (for Shape Painter)

<img src="https://resources.gdevelop-app.com/assets/Icons/checkbox-marked.svg" class="extension-icon"></img>
Checkbox that can be toggled by a left-click or touch.

**Authors and contributors** to this experimental extension: [VictrisGames](https://gd.games/VictrisGames), [D8H](https://gd.games/D8H).

---

Users can click on the checkbox to add and remove the checkmark. 

How to use:

- Add this extension to a shape painter object
- Use condition "Is checked" to find out the state of the checkbox

Tips:

- Checkbox state can also be changed by an action.
- Checkbox can be disabled so that users cannot interact with it 
- To remove halo, Set "halo hover" and "halo pressed" opacity to 0

!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.



## Checkbox 

Checkbox that can be toggled by a left-click or touch. 

### Behavior actions

**Border thickness of checkbox**  
Change the border thickness of checkbox.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Track thickness

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetBorderThickness`.

**Check (or uncheck) the checkbox**  
Check (or uncheck) the checkbox.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (❓ Yes or No): Check the checkbox?

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetChecked`.

**Enable interactions with checkbox**  
Enable or disable interactions with the checkbox. Users cannot interact while it is disabled.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (❓ Yes or No): Enable

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetEnabled`.

**Halo opacity when hovered**  
Change the halo opacity when hovered.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Halo opacity

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetHaloOpacityHover`.

**Halo opacity when pressed**  
Change the halo opacity when pressed.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Halo opacity

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetHaloOpacityPressed`.

**Halo radius when hovered**  
Change the halo radius when hovered. This size is also used to detect interaction with the checkbox.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Halo radius

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetHaloRadiusHover`.

**Halo radius when pressed**  
Change the halo radius when pressed.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Halo radius

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetHaloRadiusPressed`.

**Line width of checkmark**  
Change the line width of checkmark.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Line width (px)

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetLineWidth`.

**Primary color of checkbox**  
Change the primary color of checkbox.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (color): Primary color

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetPrimaryColor`.

**Secondary color of checkbox**  
Change the secondary color of checkbox.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (color): Secondary color

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetSecondaryColor`.

**Side length of checkbox**  
Change the side length of checkbox.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior
    - Parameter 2 (🔢 Number): Track width (px)

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::SetSideLength`.

**Toggle checkmark**  
If checked, change to unchecked.  If unchecked, change to checked.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Checkbox::Checkbox::ToggleChecked`.

### Behavior conditions

**Checkbox is being pressed**  
Check if the checkbox is being pressed by mouse or touch.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `Checkbox::Checkbox::IsBeingPressed`.

**Is checked**  
Check if the checkbox is checked.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `Checkbox::Checkbox::IsChecked`.

**Interactions enabled**  
Check if the checkbox interations are enabled.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🧩 Behavior

    > Technical note: parameter 2 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `Checkbox::Checkbox::IsEnabled`.

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.Checkbox::BorderThickness()` | Return the border thickness of checkbox (pixels). ||
| `Object.Checkbox::HaloOpacityHover()` | Return the opacity of the halo when the mouse is hovering near the checkbox. ||
| `Object.Checkbox::HaloOpacityPressed()` | Return the opacity of the halo while the checkbox is touched or clicked. ||
| `Object.Checkbox::HaloRadiusHover()` | Return the radius of the halo when the mouse is hovering near the checkbox. ||
| `Object.Checkbox::HaloRadiusPressed()` | Return the radius of the halo while the checkbox is touched or clicked. ||
| `Object.Checkbox::LineWidth()` | Return the line width of checkmark (pixels). ||
| `Object.Checkbox::PrimaryColor()` | Return the color used to draw the outline of the checkbox (when unchecked) and the fill color (when checked). ||
| `Object.Checkbox::SecondaryColor()` | Return the color used to fill the checkbox (when unchecked) and to draw the checkmark (when checked). ||
| `Object.Checkbox::SideLength()` | Return the side length of checkbox (pixels). ||


---

*This page is an auto-generated reference page about the **Checkbox (for Shape Painter)** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).