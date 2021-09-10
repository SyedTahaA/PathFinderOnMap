# PathFinderOnMap

## Run on heroku:

[Click me](https://mappingpath.herokuapp.com/)

## Run on mybinder: 

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SyedTahaA/PathFinderOnMap/mainurlpath=voila%2Frender%2Fpath_app.ipynb)

## Run locally:

cd into folder then,

```bash
  $ pip install -r requirements.txt
  $ voila --enable_nbextensions=True --theme=dark ./path_app.ipynb
```

## Introduction:

This project is an application of several pathfinding algorithms applied to real maps. The app allows one to visualize the process of the finding the path. And it further allows one to compare and contrast the differences in stats for each algortithm.

## How to use:

![Gif](https://github.com/SyedTahaA/PathFinderOnMap/blob/main/images/pathfinding.gif "Gif of using app")

  1. Type in an address (e.g. Budapest, Pest megye, Hungary) or a place (e.g. University of Toronto) to load that locations nodes and edges into the map
         Note: Larger cities can take a long time to load while smaller ones load within a few seconds.
  2. Once the map is loaded, a node will represent each intersection, while a road between two intersections is represented by edges
  3. You can select a pathfinding algorithm and hit visualize to draw the path and see the nodes traversed
  4. To compare different pathfinding algorithms, you can change the node and path color
  5. Hit the clear map button to delete previously drawn visualizations

## Algorithms:

  - Dijkstra:

        - Guarantees shortest path

        - Favours shortest weighted neighbours (minimal distance)

        - Limited to 6000m due to long find time for large distances

  - A* Search:

        - Faster version of Dijsktra

        - Guarantees shortest path

        - Favours shortest weighted neighbours (minimal distance + admissible heuristic function)

        - Haversine function is used as heuristic

  - Unsafe A* Search:

        - Doesn't guarantee shortest path

        - Similar to A* search but faster since it uses an unsafe heuristic function

  - Breadth-first Search:

         - Doesn't guarantee shortest path
         
         - Can go to any neighbouring node equally

         - Limited to 6000m due to long find time for large distances

### TODOS:

  - Improve website (Voila styling)

  - Fix drawing of non-straight eges

  

