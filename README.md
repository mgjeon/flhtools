# flhtools

```
mamba create -n flh
mamba activate flh
mamba install python ipykernel ipywidgets
mamba install numpy scipy matplotlib
```

## input

- netcdf file
    - datacube of 3D arrays $B_x$, $B_y$, $B_z$ defined at grid points of a regular grid (not on a staggered grid)


## field line tracing

- `fastfl.f90` (entire field line path)
- `fastflh.f90` (field-line helicity)

- Fortran
    - [gfortran](https://fortran-lang.org/learn/os_setup/install_gfortran/#linux)
    - [fortls](https://fortls.fortran-lang.org/quickstart.html)

## `flhcart.BField`

Python class for a 3d magnetic field snapshot on a staggered Cartesian grid

- bx
- by
- bz

- ax
- ay
- ax

- bpx
- bpy
- bpz

- apx
- apy
- apz

- computeA0Coulomb
- computeADeVore

- computeBfromA

- ghostB

- trace

- flHelicity

- computePotentialField

- poisson2dNeumann

- matchPotentialGauge

- lapMatrix

- boundaryDiv

- matchUniversalGauge

- relativeHelicity

- totalHelicity

- crossHelicity