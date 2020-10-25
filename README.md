# x16-rally-track-editor
What you need for making your own tracks for Rally Speedway

1. Download Tiled Map Editor at https://www.mapeditor.org/

2. Place the file "tiled-rallytracks-extension.js" in the extension folder. Here is where you find it:
Windows: C:/Users/<USER>/AppData/Local/Tiled/extensions/
macOS: ~/Library/Preferences/Tiled/extensions/
Linux: ~/.config/tiled/extensions/

3. Load tracks.tmx in Tiled and use this as a template for your own tracks. The file contains a map with five layers, each layer represent a track.

4. Edit the tracks. 
Change the name of the layer to change the name of the track.

Change the properties "Horizontal Start Block" and "Vertical Start Block" to state where the track begins.The upper left corner is 0,0, the lower right corner is 31,31. At the beginning of the track either a horizontal or a vertical start/finish block must be placed. A horizontal block means cars will start driving east, a vertical means they will start driving north.

Each track must have a contiguous route. In crossings without arrows the route will continue straight ahead. Note that this does not mean that the track must start and end at the same block. It can end elsewhere. You can also add multiple start/finish blocks away from the route. The player will be able to finish the race by reaching them after driving the distance of the default route.

The maps that hold your tracks are infinite. This means that if cars are going over the edge they will turn up on the exact opposite location. With help of this you can for example create an illusion of very extensive tracks. "Texas Roadtrip" is an example of this.

4. Export the map in the format "Rally Speedway Tracks". Name it tracks.bin.

5. Replace the game file tracks.bin with your file.

6. Start the game. Your tracks will be loaded and verified. If a contigous route is missing for some of the tracks, you will get an error message pointing out the exact location of the problem.
