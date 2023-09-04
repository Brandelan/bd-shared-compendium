# foundry-map-gen

## QuickStart

There is a temp button on the user list in the bottom left of the foundry window that will launch the popup

From the popup, choose your desired width/height. These are how many tiles wide/tall the map should be.

> NOTE: Small tile numbers seem to operate strangely, just stick to the defaults for now

The **Seed** value determines the random layout of the map.

**Preview** generates a thumbnail to view the map

**Generate Map** actually builds the map in the current scene. It will destroy all existing walls, and resize the scene. A popup to save the background image will appear. Save this then uploade it in the scene configuration

## Installation and Building

**Gulp Commands**: To do various build tasks via gulp, execute the following commands (configurations are in foundryconfig.json):

```

    gulp publish -u 0.1.2 : builds and updates manifest to specifies version

    gulp build : builds everything from the 'src' folder to a 'dist' folder

    gulp link : builds everything from 'src' to the specified foundry directory

    gulp link --clean : remove the link to the foundry vtt folder

    gulp clean : removes all files from the dist folder
```

**Git Repos**

There is a map generator git repo this package uses. to install the first time run:

```
    npm run clonelibs
```

To update the file you can run:

```
    npm run pullLibs
```

or just navigate to the folder and do a regular git pull

## v0.1.2

Tweaked some internal publishing stuff. Testing out publishing via gulp, not really a **true** update

## v0.1.1

Updated the map generator to work with Foundry v.0.8.8

## v0.1.0

Initial release.

This module is designed to be used with
Foundry Virtual TableTop, (any) Edition.

This module adds a some procedural dungeon generation abilities to foundry.
