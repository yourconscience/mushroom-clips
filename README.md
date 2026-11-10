# mushroom-clips

Audio for [ГРИБ: Versus](https://github.com/yourconscience/mushroom): 400 fifteen-second clips and `manifest.json`.

The game fetches them from `https://yourconscience.github.io/mushroom-clips/`, one clip per zone. They live apart from the game so that a game release does not re-upload 96 MB.

`manifest.json` is `{"files": [...], "t": [...]}`; `t` holds the titles XOR-ed with a fixed key and base64-encoded. `tools/cut-clips.py` in the game repo writes both the clips and the manifest.
