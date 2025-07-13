## CUDA

CUDA (Compute Unified Device Architecture) [is a parallel computing platform and programming model developed by NVIDIA for general computing on graphical processing units (GPUs)](https://developer.nvidia.com/cuda-zone).
The CUDA ecosystem provides software developer software development kits (SDK) with APIs to CUDA that allow for software developers to write hardware accelerated programs with CUDA in various languages for NVIDIA GPUs.
CUDA has official language support for C++, Fortran, and Python, with community support for Julia.
While there are other types of hardware acceleration development platforms, as of 2025 CUDA is the most abundant platform for scientific computing that uses GPUs and effectively the default choice for major machine learning libraries and applications.

CUDA is closed source and proprietary to NVIDIA, which means that NVIDIA has historically limited the download access of the CUDA toolkits and drivers to registered NVIDIA developers (while keeping the software free (monetarily) to use).
CUDA then required a [multi-step installation process](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/) with manual steps and decisions based on the target platform and particular CUDA version.
This meant that when CUDA enabled environments were setup on a particular machine they were powerful and optimized, but brittle to change and could easily be broken if system wide updates (like for security fixes) occurred.
CUDA software environments were bespoke and not many scientists understood how to construct and curate them.

### CUDA on conda-forge

In [late 2018](https://github.com/conda-forge/conda-forge.github.io/issues/687) to better support the scientific developer community, NVIDIA started to release components of the CUDA toolkits on the [`nvidia` conda channel](https://anaconda.org/nvidia).
This provided the first access to start to create conda environments where the versions of different CUDA tools could be directly specified and downloaded.
However, all of this work was being done internally in NVIDIA and as it was on a separate channel it was less visible and it still required additional knowledge to work with.
In [2023](https://youtu.be/WgKwlGgVzYE?si=hfyAo6qLma8hnJ-N), NVIDIA's open source team began to move the release of CUDA conda packages from the `nvidia` channel to conda-forge, making it easier to discover and allowing for community support.
With significant advancements in system driver specification support, CUDA 12 became the first version of CUDA to be released as conda packages through conda-forge and included all CUDA libraries from the [CUDA compiler `nvcc`](https://github.com/conda-forge/cuda-nvcc-feedstock) to the [CUDA development libraries](https://github.com/conda-forge/cuda-libraries-dev-feedstock).
They also released [CUDA metapackages](https://github.com/conda-forge/cuda-feedstock/) that allowed users to easily describe the version of CUDA they required (e.g. `cuda-version=12.5`) and the CUDA conda packages they wanted (e.g. `cuda`).
This significantly improved the ability for researchers to easily create CUDA accelerated computing environments.


* Overview of CUDA 12 packages
* Importance of the work
* What it enables
