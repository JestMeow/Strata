# strata
An addon for Minecraft: Bedrock Edition that helps you build large organic shapes effeciently using brush tools and commands.

## Features
- Brush-based terrain editing
- Sphere, cylinder, and cuboid brushes
- Replace and fill blocks
- Melt, fill, and smooth areas

# Installation
1. Download the latest release or the addon version that supports your Minecraft version.
2. Import the `.mcaddon` file.
3. Activate the behaviour pack in your world.
4. Enable beta API experimental feature.
5. Start the world.

## Usage
### Commands
The command prefix for this addon is ```>```.

1. config, c
   - Configures the addon settings. Available option is ```optimize```. If true, brushes will generate shapes in layers with delay. This can slow up the building process, but reduces lag spikes.
2. brush, b
   | Subcommands | Description | Additional description/Example |
   |---|---|---|
   | slot ```[int]``` | Sets the brush slot to the inventory slot with id ```[int]``` | ```>slot 8``` sets the brush slot to the **9th** hotbar slot. If the brush is on normal mode, it will fill using whatever block is in this slot. If the slot is empty, it will simply fill with stone.|
   | shape / sh ```[shape]``` | Sets the brush shape to ```[shape]```. Shape can be cuboid ```cuboid```, sphere ```sphere/ball/b```, or cylinder ```cylinder/cyl/disk/d```. |
   | size / sz ```[width/radius]``` ```[height``` | Sets the dimensions of the brush. | If brush shape is sphere and height is left empty, then height will be automatically set to 1. |
   | mode normal / m n | Sets the brush mode to normal | Fills shape with blocks. |
   | mode erosion melt / m e melt | Sets the brush mode to melt | Removes **some** blocks in an area. |
   | mode erosion fill / m e fill | Sets the brush mode to fill | Fills **some** blocks in an area. |
   | mode erosion smooth / m e smooth | Sets the brush mode to smooth. | Smooths an area. |
   | mode overlay / m o ```[depth]```| Sets the brush mode to overlay. | Only replaces the top layer of blocks in an area with. ```depth``` is the depth in blocks. |
   | mode paint / m p | Sets the brush mode to paint. | Replaces non-air blocks with blocks. |

## Compatibility
This addon should work with most other addons. It is recommended to use this addon along with [Bliding Staf](https://github.com/JestMeow/Bliding-Staf).
