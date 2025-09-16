# 3D camera shake

<img src="https://resources.gdevelop-app.com/assets/Icons/vector-difference-ab.svg" class="extension-icon"></img>
Shake 3D layer cameras.

**Authors and contributors** to this experimental extension: [D8H](https://gd.games/D8H).

!!! warning
    This is an extension made by a community member and it only got through a
    light review by the GDevelop extension team. As such, we can't guarantee it
    meets all the quality standards of fully reviewed extensions.

---

Shake layer cameras on 3 rotations.


- Short shaking can be used to give impact (explosion, hit)
- Shaking can go indefinitely to set an ambiance (engine vibration, earthquake, pulsing)
- Low frequency shaking allows to simulate slow moving objects (ship rocking back and forth)


!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.

## Actions

**Horizontal rotation amplitude**  
Change the horizontal rotation amplitude of the shaking (in degrees).

**Shakable layer**  
Mark a layer as shakable.

**Layer shaking frequency**  
Change the number of back and forth per seconds.

**Spinning shake amplitude**  
Change the spinning amplitude of the shaking (in degrees).

**Vertical rotation amplitude**  
Change the vertical rotation amplitude of the shaking (in degrees).

**Shake camera**  
Shake the camera on layers chosen with configuration actions.

**Start camera shaking**  
Start shaking the camera indefinitely.

**Stop camera shaking**  
Stop shaking the camera.

## Conditions

**Horizontal rotation amplitude**  
Compare the horizontal rotation amplitude of the shaking (in degrees).

**Camera is shaking**  
Check if the camera is shaking.

**Spinning shake amplitude**  
Compare the spinning amplitude of the shaking (in degrees).

**Vertical rotation amplitude**  
Compare the vertical rotation amplitude of the shaking (in degrees).

## Expressions

| Expression | Description |  |
|-----|-----|-----|
| `CameraShake3D::HorizontalAmplitudeAngle(layer name)` | Return the horizontal rotation amplitude of the shaking (in degrees). ||
| | _🔤 Layer name (String)_ | Layer |
| `CameraShake3D::SpineAmplitudeAngle(layer name)` | Return the spinning amplitude of the shaking (in degrees). ||
| | _🔤 Layer name (String)_ | Layer |
| `CameraShake3D::VerticalAmplitudeAngle(layer name)` | Return the vertical rotation amplitude of the shaking (in degrees). ||
| | _🔤 Layer name (String)_ | Layer |


---

*This page is an auto-generated reference page about the **3D camera shake** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).