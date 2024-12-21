# Advanced movements for 3D physics characters

<img src="https://resources.gdevelop-app.com/assets/Icons/Line Hero Pack/Master/SVG/Sports and Fitness/Sports and Fitness_training_running_run.svg" class="extension-icon"></img>
Let 3D physics characters: air jump, wall jump wall sliding, coyote time and dashing.

**Authors and contributors** to this community extension: [D8H](https://gd.games/D8H), [shadow00dev](https://gd.games/shadow00dev), [Entropy](https://gd.games/Entropy), [CorianderGames](https://gd.games/CorianderGames).

---

This extension provides behaviors to:


* Jump in mid-air
* Do coyote time, also known as "ledge tolerance". It lets players jumping even after their character is no longer touching the ground for a given amount of time. It aims to give players a feeling of control and reduce frustration.

!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.



## Coyote time and air jump for 3D 

Let 3D physics characters jump shortly after leaving a platform and also jump in mid-air. 

### Behavior actions

**Remove a remaining air jump**  
Remove one of the remaining air jumps of a character.

**Reset air jumps**  
Allow back all air jumps of a character.

**Air jumps**  
Change the number of times the character can jump in mid-air.

**Coyote timeframe**  
Change the coyote time duration of an object (in seconds).

### Behavior conditions

**Floor jumps count as air jumps**  
Check if floor jumps are counted as air jumps for an object.

**Can coyote jump**  
Check if a coyote jump can currently happen.

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.AdvancedJump3D::AirJumpsMax()` | Number of jumps in mid-air that are allowed. ||
| `Object.AdvancedJump3D::RemainingAirJumps()` | Number of jumps in mid-air that are still allowed. ||

---

*This page is an auto-generated reference page about the **Advanced movements for 3D physics characters** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).