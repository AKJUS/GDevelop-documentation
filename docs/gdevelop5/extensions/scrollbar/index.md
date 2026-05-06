# Scrollbar

<img src="https://asset-resources.gdevelop.io/public-resources/Icons/Line Hero Pack/Master/SVG/Interface Elements/c1313ac0735bd1c08d7327fd9a56b4d8cebf1b343f9ba82f1b141358433e1cdb_Interface Elements_interface_ui_scroll_bar_scrollbar.svg" class="extension-icon"></img>
A scrollbar to help making a scroll view.

**Authors and contributors** to this experimental extension: [D8H](https://gd.games/D8H), [Jurfix](https://gd.games/Jurfix), [Alios](https://gd.games/Alios).

!!! warning
    This is an extension made by a community member and it only got through a
    light review by the GDevelop extension team. As such, we can't guarantee it
    meets all the quality standards of fully reviewed extensions.

---

A scrollbar to help making a scroll view.

An example of scroll view can be found in the [multiplayer custom lobbies](https://wiki.gdevelop.io/gdevelop5/extensions/multiplayer-custom-lobbies/) extension.

!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.

## Actions

**Set camera from scroll**  
Move the camera according to the scroll position.

??? quote "See parameters & details"

    - Parameter 1: 👾 Object
    - Parameter 2 (🔤 Layer name (String)): Scrolled layer

    > Technical note: parameters 0, 3 are internal parameters handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Scrollbar::SetCameraFromPosition`.

**Set scroll from camera**  
Change the scroll position according to the camera.

??? quote "See parameters & details"

    - Parameter 1: 👾 Object
    - Parameter 2 (🔤 Layer name (String)): Scrolled layer

    > Technical note: parameters 0, 3 are internal parameters handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Scrollbar::SetPositionFromCamera`.




## Scrollbar 

A scrollbar to help making a scroll view. 

### Object properties

- **Min thumb length** (🔢 Number, Distance). Default value is `40`.
- **Hide the bar when the content is too small** (🔘 Boolean). Default value is `true`.

??? quote "See internal technical details"


    - **Min thumb length** is stored as `ThumbLengthMin` (Number). Unit is Pixel. Default value is `40`.
    - **Hide the bar when the content is too small** is stored as `ShouldHideWhenUseless` (Boolean). Default value is `true`.

### Object actions

**Content length**  
Change the content length of the object. The length of the content to scroll. The scroll bar don't actually scroll the content. You have to do it yourself with camera actions.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Operator
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Scrollbar::Scrollbar::SetContentLength`.

**Scroll position**  
Change the top or left position of the displayed part.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Operator
    - Parameter 2 (🔢 Number): Value

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this action internal type (in GDevelop JSON) is `Scrollbar::Scrollbar::SetScrollPosition`.


### Object conditions

**Content length**  
Compare the content length of the object. The length of the content to scroll. The scroll bar don't actually scroll the content. You have to do it yourself with camera actions.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Relational operator
    - Parameter 2 (🔢 Number): Value to compare

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `Scrollbar::Scrollbar::ContentLength`.

**Scrolling is required**  
Check if the content is big enough to require scrolling.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object

    > Technical note: parameter 1 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `Scrollbar::Scrollbar::IsScrollingRequired`.

**Thumb is dragged**  
Check if the thumb of the scrollbar is dragged.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object

    > Technical note: parameter 1 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `Scrollbar::Scrollbar::IsThumbDragged`.

**Scroll position**  
Compare the top or left position of the displayed part.

??? quote "See parameters & details"

    - Parameter 0: 👾 Object
    - Parameter 1: 🟰 Relational operator
    - Parameter 2 (🔢 Number): Value to compare

    > Technical note: parameter 3 is an internal parameter handled by GDevelop.

    > Technical note: this condition internal type (in GDevelop JSON) is `Scrollbar::Scrollbar::ScrollPosition`.


### Object expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.ContentLength()` | Return the content length of the object. The length of the content to scroll. The scroll bar don't actually scroll the content. You have to do it yourself with camera actions. ||
| `Object.ScrollPosition()` | Return the top or left position of the displayed part. ||


---

*This page is an auto-generated reference page about the **Scrollbar** extension for [GDevelop, the open-source, AI-powered, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop extensions here](/gdevelop5/extensions).