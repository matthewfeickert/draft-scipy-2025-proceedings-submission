## Introduction

A critical component of research software sustainability is the reproducibility of the software and computing environments software operates and "lives" in.
Providing software as a "package" &mdash; a standardized distribution of all source or binary components of the software required for use along with identifying metadata &mdash; goes a long way to improved reproducibility of software libraries.
However, more researchers are consumers of libraries than developers of them, but still need reproducible computing environments for research software applications that may be run across multiple computing platforms &mdash; e.g. scientific analyses, visualization tools, data transformation pipelines, and artificial intelligence (AI) and machine learning (ML) applications on hardware ac:1celerator platforms (e.g. GPUs).
While workflow engines and Linux containers offer a gold standard for scientific computing reproducibility, they require additional layers of training and software engineering knowledge.
Modern open source multi-platform environment management tools, e.g. [@pixi], provide automatic multi-platform hash-level lock file support for all dependencies &mdash; down to the compiler level &mdash; of software on public package indexes (e.g. PyPI [@PyPI_website] and conda-forge [@conda-forge_community]) while still providing a high level interface well suited for researchers.
Combined with the arrival of the full CUDA [@CUDA_paper] stack on conda-forge, it is now possible to declaratively specify a full CUDA accelerated software environment.
We are now at a point where well supported, robust technological solutions exist, even for applications with highly complex software environments.
What is currently lacking is the education and training by the broader scientific software community to adopt these technologies and build community standards of practice around them, as well as an understanding of what are the most actionably useful features of adopting computational reproducibility tools.

## Reproducibility

"Reproducible" research can mean many things and is a multipronged problem.
Focus primarily on computational reproducibility.
Like all forms of reproducibility, there are multiple "levels" of reproducibility.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum sapien
tortor, bibendum et pretium molestie, dapibus ac ante. Nam odio orci, interdum
sit amet placerat non, molestie sed dui. Pellentesque eu quam ac mauris
tristique sodales. Fusce sodales laoreet nulla, id pellentesque risus convallis
eget. Nam id ante gravida justo eleifend semper vel ut nisi. Phasellus
adipiscing risus quis dui facilisis fermentum. Duis quis sodales neque. Aliquam
ut tellus dolor. Etiam ac elit nec risus lobortis tempus id nec erat. Morbi eu
purus enim. Integer et velit vitae arcu interdum aliquet at eget purus. Integer
quis nisi neque. Morbi ac odio et leo dignissim sodales. Pellentesque nec nibh
nulla. Donec faucibus purus leo. Nullam vel lorem eget enim blandit ultrices.
Ut urna lacus, scelerisque nec pellentesque quis, laoreet eu magna. Quisque ac
justo vitae odio tincidunt tempus at vitae tortor.

* Introduction
* Computational reproducibility
* Computational reproducibility vs. scientific reuse
