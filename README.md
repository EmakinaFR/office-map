# Office map

This is a repo to recreate our offices in a living pixel map using [WorkAdventure](https://workadventu.re).

## Tools you will need 🛠

In order to be able to edit and contribute to the maps, you need:

- the [Tiled editor](https://www.mapeditor.org/) software
- "tiles" (i.e. images) to create your map. Those images are the material to create maps (with objects, floors, etc.). 
  They contain tiles (squares of 32x32 pixels) which can be placed on the map. There are several tilesets from the starter
  kit, and a custom one (tileset_custom.png) that gathers custom tiles.

## Getting started 🚀

Clone the repo :

```bash
git clone https://github.com/EmakinaFR/office-map 
```

Open the Tiled software.

### Loading the map in Tiled 📦

The Limoges office map is in the file `map.json`.

The Paris office map is in the file `map-paris.json`.  

You can load these files in [Tiled](https://www.mapeditor.org/).

Some resources regarding Tiled:

- [Tiled documentation](https://doc.mapeditor.org/en/stable/manual/introduction/)
- [Tiled video tutorials](https://www.gamefromscratch.com/post/2015/10/14/Tiled-Map-Editor-Tutorial-Series.aspx)

### WorkAdventu.re documentation 📖 

**Everything you need to know to create or edit a map is described in the [WorkAdventure documentation](https://workadventu.re/map-building).**
Please be sure to check it out. 

#### Layers

To properly display objects above other objects or floor, we use layers, like in Photoshop for example. 
When adding or editing a map, be sure to respect the right layer order.

For example :

- **objects level 2** : this layer will host objects (computers) that are displayed above the desks
- **objects level 1** : this layer will host objects (desks) that are displayed above the floor
- **floor** : this layer will host floor tiles

#### Custom tileset

For custom objects, there is a custom tileset called `tileset_custom.png`.
Add any new tile into this tileset if needed, using Affinity Photo and the `tileset_custom.aphoto` source file.
Commit this source file too.

### Pushing the map 🌐

When your changes are ready, commit and push the changes back to GitHub.

```bash
git add .
git commit -m "Add good vibes in the office"
git push origin feature/my-branch 
```

Open a pull request to merge your changes.

Once merged into the master branch, the map will be propagated automatically within minutes to the GitHub pages web-server.
