# cub3D
![image](https://github.com/fsemke/cub3D/assets/94831163/d3b59fa9-4a09-4c53-acbc-fb5bd9d07024)

This is a Raycaster project, created for the 42 cursus.
It's written in C with the miniLibX library.

## Requirements
A Linux system and the necessary packages:
```sudo apt install build-essential libx11-dev libglfw3-dev libglfw3 xorg-dev```

## How to compile it
run ```make all``` to compile this project.

## How to run it
Choose one map and run it with:
```./cub3d maps/map1.cub```

## Controls
```W``` Move forward

```A``` Move left

```S``` Move back

```D``` Move right

```Left``` Look to the left

```Right``` Look to the right

```ESC``` Close the game


## Create own maps
You can also create own maps.

The rules for the map:

```NO <PATH>``` Path to the texture for the North wall

```WE <PATH>``` Path to the texture for the West wall

```EA <PATH>``` Path to the texture for the East wall

```SO <PATH>``` Path to the texture for the South wall

```F <RGB in format 255,255,255>``` The color for the floor

```C <RGB in format 255,255,255>``` The color for the ceiling

And the map itself:

```
1111
10N1
1111
```

```1``` wall

```0``` empty space

```N``` spawn in north direction

```S``` spawn in south direction

```W``` spawn in west direction

```E``` spawn in east direction

But don't worry, our game won't crash if the map has an error.
