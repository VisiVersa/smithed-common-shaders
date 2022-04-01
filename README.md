# Common Shaders
 Vanilla Minecraft shaders for various effects, merged into one pack.

# Marker particle tints
Preferably, setting the red channel to be 254 or 253 sets it to be a marker, and the green channel identifies which effect you choose.
* (254, 253, x): Manic

# Marker pixel screen positions
To ensure that all packs can receive their inputs simultaneously, marker particles are transformed to fill different screen positions. They should form a gridlike pattern to make it possible to reconstruct every pixel from its surroundings.
* (0, 0): Manic

# Fabulous shader common.data buffer layout
* Row 0: Pixel 0 contains time since last shader reload, read as `time = dataTime.x + 255. * dataTime.y + 65025. * dataTime.z;` to get the value in seconds.
* Row 1: Manic

# Core shaders included from other repositories
* https://github.com/Ancientkingg/fancyPants
* https://github.com/ShockMicro/CorePerspectiveModels
* https://github.com/ShockMicro/VanillaDynamicEmissives
