## Conda packages

Conda packages (`.conda` files) are language agnostic file archives that contain built code distributions and metadata.
This is quite powerful, as it allows for arbitrary code to be built for any target platform and then packaged with its metadata.
When a conda package is downloaded and then unpacked with a conda package management tool (e.g. Pixi, conda, mamba) it is then "installed" by copying the package's file directory tree to the base of the environment's directory tree.
Package contents are also simple; they can only contain files and symbolic links.

### conda-forge

Technical overview of conda-forge and conda packages.
