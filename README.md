## Installation

1. Use micromamba to create an environment with Python 3.11: `micromamba create -n stl-repair`, `micromamba activate stl-repair`, `micromamba install python==3.11`, & `pip install .` (in the cloned dir).
2. Blender needs to be installed, and the `object_print3d_utils` add-on must be installed. I found it [in this collection on github](https://github.com/sobotka/blender-addons). The relevant directory must be zipped and then installed through the Blender gui. I may upload the zip here.
3. Optionally `ln -s ~/.local/share/mamba/envs/stl-repair/bin/repair_stls ~/.local/bin/repair_stls`.


## Usage

```console
$ repair_stls [OPTIONS] FILEPATH
```

**Arguments**:

* `FILEPATH`: The path to either a single STL file to repair or a directory full of stls  [required]

**Options**:

* `-o, --output PATH`: Where to write repaired files to  [required]
* `-s, --suffix TEXT`: Suffix to append to output files  [default: _fixed]
* `--debug`: Print extra information for debugging.
* `--version`: Print version number.
* `--help`: Show this message and exit.
