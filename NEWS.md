# SpatialGEV 1.0.2

* Mesh generation for `kernel = "spde"` now uses `fmesher::fm_mesh_2d_inla()`
  instead of the deprecated `INLA::inla.mesh.2d()`.
* Added an element-wise `pow()` so the package compiles against Eigen 5.0
  (upcoming RcppEigen).
* `spatialGEV_fit()` gains a maximum step argument and a default prior on `s`
  for `method = "maxsmooth"`; `data` may again be a list of estimates and
  variances for that method.
* Fixed `spatialGEV_predict()` for model "a" with a single test location.
* Added the `simulatedData_withcov` dataset and covariate instructions in the
  vignette.
* Extended unit tests; the vignette is now precompiled.
* Updated the package reference to Chen, Ramezan, and Lysy (2024),
  <doi:10.1002/cjs.11829>.

# SpatialGEV 1.0.1

* Initial CRAN release.
