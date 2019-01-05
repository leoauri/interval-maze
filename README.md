# Interval Maze
Build mazes with depth first search algorithm, in a specified number of dimensions.  
Use the mazes to generate melodies, where higher dimensions correspond to larger intervals.
Listen to renderings of the generated melodies with [music21 library](https://github.com/cuthbertLab/music21).

The [Jupyter Notebook](https://github.com/leoauri/interval-maze/blob/master/Interval%20Maze.ipynb) contains more notes, diagrammes and examples.

## Installation
- clone repo
- `cd` into directory
- `pipenv install`
- run notebook in environment: `pipenv run jupyter notebook`
- install MuseScore to see scores, for example with `brew cask install musescore`

In case of a problem where music21 has a misconfigured path to MuseScore, this snippet may solve it:
```
path = '/Applications/MuseScore 3.app/Contents/MacOS/mscore'

import music21
import pathlib

music21.environment.set('musicxmlPath', pathlib.PosixPath(path))
music21.environment.set('musescoreDirectPNGPath', pathlib.PosixPath(path))
```
