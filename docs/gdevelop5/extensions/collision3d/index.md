# 3D collision

<img src="https://asset-resources.gdevelop.io/public-resources/Icons/7a5696a515bf40813692e118147568392a854f65f5b50750c9b9aaa967aba7df_vector-intersection.svg" class="extension-icon"></img>
Check collision and distance between 3D objects.

**Authors and contributors** to this community extension: [D8H](https://gd.games/D8H), [TulenvakiProductions](https://gd.games/TulenvakiProductions).

!!! warning
    This is an extension made by a community member — but not reviewed
    by the GDevelop extension team. As such, we can't guarantee it
    meets all the quality standards of official extensions. In case of
    doubt, contact the author to know more about what the extension
    does or inspect its content before using it.

---

Check collision and distance between 3D objects and separate them from each other.

!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.

## Actions

**Separate objects in 3D**  
Move an object away from another using their collision masks. Object rotation around X and Y axes are ignored.  
Be sure to call this action on a reasonable number of objects to avoid slowing down the game.

## Conditions

**Collision in 3D**  
Check the collision between two objects using their collision masks. Object rotation around X and Y axes are ignored.

**Distance between two objects in 3D**  
Compare the distance between two objects in 3D.

**Pick nearest object in 3D**  
Pick the object of this type that is nearest to the specified position in 3D.

## Expressions

| Expression | Description |  |
|-----|-----|-----|
| `Collision3D::Distance()` | Distance between two objects in 3D. ||
| `Collision3D::DistanceToPosition()` | Distance between an object and a position in 3D. ||
| `Collision3D::SqDistance()` | Square distance between two objects in 3D. ||
| `Collision3D::SqDistanceToPosition()` | Square distance between an object and a position in 3D. ||

---

*This page is an auto-generated reference page about the **3D collision** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).