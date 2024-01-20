## [Getting started with Raspberry Pi Pico C/C++](https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf)

## Ref:
- [Using Conda to Create C++ Environments](https://gist.github.com/jpz/1c33c466b9af1287abfa51497ab1c0a4)

1. Install conda
2. Create a conda environment & Activate the Virtual Env
```bash
conda create -n COMP6771
conda activate COMP6771
```
3. Install related Packages
```bash
conda install -y -c conda-forge/label/llvm_rc clangdev
conda install -y -c conda-forge abseil-ccp gsl-lite fmt catch2
