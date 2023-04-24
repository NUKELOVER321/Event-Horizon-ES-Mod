# Ships

This folder contains data files on ships.   
Most ships consist of a ship file and zero or more ship build files.   

Below is an example of a component file, followed by a description of what each data field does.

```json
{
  "ItemType": 6,
  "Id": 413,
  "ShipCategory": 1,
  "Name": "Model 8",
  "Faction": 212,
  "IconImage": "model 8 icon.png",
  "IconScale": 1.0,
  "ModelImage": "model 8.png",
  "ModelScale": 2.0,
  "EnginePosition": {
    "x": -0.96,
    "y": 0.24
  },
  "EngineColor": "#7DEF9F0F",
  "EngineSize": 0.1,
  "Engines": [
    {
      "Position": {
        "x": -0.96,
        "y": -0.21
      },
      "Size": 0.1
    }
  ],
  "Layout": "000000010000000000000114400000000000114400000000001111110000000044111110000000044222110000000111222110000001112222211100001222222222100000122222221100001112222211000000112222211000001111222110000000015525510000000015505510000",
  "Barrels": [
    {
      "Position": {
        "x": 0.7,
        "y": -0.2
      },
      "PlatformType": 3,
      "WeaponClass": "CLTM"
    },
    {
      "Position": {
        "x": 0.4,
        "y": 0.2
      },
      "PlatformType": 3,
      "WeaponClass": "CLTM"
    }
  ]
}
```

Data fields:
- `"ItemType"`: Tells the database editor program what type of data file is being read (in this case: a component file).
- `"Id"`: Unique ID assigned to this file. Each ship file must have a unique ID.
- `"Name"`: Name of the ship as displayed in-game.
- `"Faction"`: Unique ID of the faction the ship belongs to. This field can be deleted for ships not assigned to any faction.
- `"IconImage"`: Name of the image to be used for the ship's icon (preview image shown in the upper right hand corner of the game window during a battle).
- `"IconScale"`: Size of the icon image relative to the frame it is displayed in.
- `"ModelImage"`: Name of the image to be used for the ship's model.
- `"ModelScale"`: Size of the ship model.
- `"Availability"`: Number denoting the places that this ship can appear in in-game.
- `"EngineColor"`: Hex color code that determines the color of the ship's shield and engine effects.
- `"Engines"`: A list of engine trail objects.
  - `"Position"`: A tuple containing an x and y coordinates denoting the location of an engine trail effect. (0,0) is at the very center of the ship. Note that the X direction is up/down instead of left/right.
  - `"Size"`: Size of the engine trail effect.
- `"Layout"`: A bunch of digits representing the unrolled version of a square of digits denoting the cell layout of the ship. The number of digits must be a square of some number. It is better to modify this using the database editor instead of by hand due to the ease of modification.
- `"Barrels"`: A list of barrel objects. Each barrel denotes a location where a weapon can spawn projectiles from.
  - `"Position"`: See the data field of the same name in the Engines section.
  - `"PlatformType"`: A value denoting the type of barrel at this location. Each type gives the barrel a different amount of aim assist.
  - `"WeaponClass"`: A string containing all the weapon slot types that this barrel accepts.