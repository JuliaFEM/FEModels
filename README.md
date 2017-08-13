# FEModels

Finite Element test models library contains finite element meshes which can
then be used in examples and to measure performance of code.

Use `FEModels.jl` to download models easily for your working directory:
```julia
using FEModels
dirname = "block-and-cylinder"
meshname = "mesh_sparse.inp"
fe_download(dirname, meshname)
```

Now, you should have mesh file in your working directory:

    ./block-and-cylinder/mesh_sparse.inp

## Guides for adding new models

- Compress model using maximum compression, e.g. `gzip2 -9 model.inp` or similar.
- Include step or geometry, if possible, so that new meshes can be generated if needed.
- Include pictures of meshes, models, surface sets and node sets if possible.
- Write README.md to the directory where you can describe model more if needed.
- It's nice to mention where model is downloaded and who has made it.
- Make sure that model can be used for non-commercial purposes.
