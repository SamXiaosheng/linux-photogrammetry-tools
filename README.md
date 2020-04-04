# linux-photogrammetry-tools
![build](https://github.com/epassaro/linux-photogrammetry-tools/workflows/build/badge.svg)

A set of photogrammetry tools compiled for Ubuntu 18.04 and ready to use:

- SIFT by [vlfeat.org](https://www.vlfeat.org/)
- [Bundler](https://github.com/snavely/bundler_sfm) (compiled with Ceres Solver) by Noah Snavely
- A patched version of `bundler.py` compatible with VLFeat SIFT (based on [Python Photogrammetry Toolbox](https://github.com/steve-vincent/photogrammetry))
- [CMVS \& PMVS2](https://github.com/pmoulon/CMVS-PMVS) by Yasutaka Furukawa


## Download
Get latest build from [here](https://github.com/epassaro/linux-photogrammetry-tools/releases/download/stable/lpt-ubuntu-18.04.tar.gz) and extract it.


## Dependencies
Probably you have most of these dependencies already installed on your system:

`build-essential` `libc6-i386` `libjpeg62` `liblapack3` `libceres1` `jhead` `python` `python-pil` `python-ruamel.yaml`


## Run example
`IMG_DIR` is set at the top of `Makefile` and pointing to the example folder by default. Just run `make` in the terminal to process the images.


## Visualize the results
Open with [Meshlab](http://www.meshlab.net/) the `.ply` file located at `work_dir/pmvs/models/`. 

Check the log file inside `work_dir` directory in case of error.

## License

Code released under the [GNU GPLv3 License](https://raw.githubusercontent.com/epassaro/linux-photogrammetry-tools/master/LICENSE).
