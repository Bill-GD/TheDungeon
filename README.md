# The Dungeon
Test game for features not in The Treasure

- Assets: [2D Dungeon Pack](https://pixel-poem.itch.io/dungeon-assetpuck)

- Planned Features (to test & might not be implemented):
  - ✅ Y-Sorting: Top-down 2D, 0° < camera angle < 90°
    - Enable ```Y Sort Enabled``` in ```CanvasItem``` tab and set ```Y Sort Origin``` correspondingly
  - ▢ Proper Lighting: Shadow behind sprite/tile
    - Normal nodes: use 2 Light nodes for light source (1 for light, 1 for shadow)
    - TileMap: impossible, shadow will always be on top of tile, occluder mask config is limited
  - ▢ Navigation: TileMap & Object (avoid external objects when navigating on tiles)
    - TileMap: use NavigationLayer and NavigationAgent for entities
    - Bodies: __manually__ draw NavigationRegion around objects (4.2 has baking)
    - TIleMap & Bodies: impossible, NavigationRegion and TileMap NavigationLayer don't work together
  - ▢ Melee attacks: Swing, Collision, Animation...
  - ▢ Object (non-TileMap) interactions: open/close chests
  - ▢ TileMap interactions: open/close doors