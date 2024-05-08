# imageSplit API Documentation.
imageSplit is a paid API that allows you to convert a string of numbers into tiles and then combines them all into an image.

## `GET` List Entire Tileset.
Lists each tile and there tile ID. <br>
address: `menzico.com/imageSplit/list/:APKIKEY/:TILESETID`

## `GET` View Specific Tile.
Returns a image of the tile. <br>
address: `menzico.com/imageSplit/list/:APKIKEY/:TILESETID/:TILEID`

## `POST` Generate an image.
Sends a number set to the API to generate an image. <br>
address: `menzico.com/imageSplit/gen/:APIKEY/:TILESETID/:TILESETCODE` <br>
number sets must be designed like the example below: <br>

for example if `1 = Grass` and `2 = Rock` and you want the first two tiles to be rocks and the rest grass in a 3x3 image you would send. 
```
2-2-1/1-1-1/1-1-1
```
