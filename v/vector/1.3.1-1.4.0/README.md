# Comparing `tmp/vector-1.3.1.tar.gz` & `tmp/vector-1.4.0.tar.gz`

## Comparing `vector-1.3.1.tar` & `vector-1.4.0.tar`

### file list

```diff
@@ -1,307 +1,373 @@
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 vector-1.3.1/.all-contributorsrc
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 vector-1.3.1/.git_archival.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 vector-1.3.1/.gitattributes
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 vector-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 vector-1.3.1/.readthedocs.yml
--rwxr-xr-x   0        0        0      887 2020-02-02 00:00:00.000000 vector-1.3.1/CITATION.cff
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 vector-1.3.1/environment.yml
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 vector-1.3.1/noxfile.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 vector-1.3.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 vector-1.3.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 vector-1.3.1/.github/codecov.yml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 vector-1.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 vector-1.3.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 vector-1.3.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 vector-1.3.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 vector-1.3.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 vector-1.3.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 vector-1.3.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 vector-1.3.1/.github/workflows/notebooks.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 vector-1.3.1/docs/Makefile
--rw-r--r--   0        0        0    13588 2020-02-02 00:00:00.000000 vector-1.3.1/docs/changelog.md
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 vector-1.3.1/docs/conf.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 vector-1.3.1/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 vector-1.3.1/docs/make.bat
--rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 vector-1.3.1/docs/_images/LogoSrc.svg
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 vector-1.3.1/docs/_images/vector-logo.png
--rw-r--r--   0        0        0   174177 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/inheritance.svg
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/modules.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/vector._methods.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/vector._typeutils.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/vector.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/backends/vector.backends._numba.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/backends/vector.backends._numba_object.rst
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/backends/vector.backends.awkward.rst
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/backends/vector.backends.awkward_constructors.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/backends/vector.backends.numba_numpy.rst
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/backends/vector.backends.numpy.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/backends/vector.backends.object.rst
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/backends/vector.backends.rst
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/vector._compute.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.Et.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.Et2.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.Mt.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.Mt2.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.add.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.beta.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.boostX_beta.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.boostX_gamma.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.boostY_beta.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.boostY_gamma.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.boostZ_beta.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.boostZ_gamma.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.boost_beta3.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.boost_p4.rst
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.deltaRapidityPhi.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.deltaRapidityPhi2.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.dot.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.equal.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.gamma.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.is_lightlike.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.is_spacelike.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.is_timelike.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.isclose.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.not_equal.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.rapidity.rst
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.scale.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.subtract.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.t.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.t2.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.tau.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.tau2.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.to_beta3.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.transform4D.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.unit.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.add.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.deltaphi.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.dot.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.equal.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.is_antiparallel.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.is_parallel.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.is_perpendicular.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.isclose.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.not_equal.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.phi.rst
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.rho.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.rho2.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.rotateZ.rst
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.scale.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.subtract.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.transform2D.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.unit.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.x.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/planar/vector._compute.planar.y.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.add.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.costheta.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.cottheta.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.cross.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.deltaR.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.deltaR2.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.deltaangle.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.deltaeta.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.dot.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.equal.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.eta.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.is_antiparallel.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.is_parallel.rst
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.is_perpendicular.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.isclose.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.mag.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.mag2.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.not_equal.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.rotateX.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.rotateY.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.rotate_axis.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.rotate_euler.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.rotate_quaternion.rst
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.scale.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.subtract.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.theta.rst
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.transform3D.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.unit.rst
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.z.rst
--rw-r--r--   0        0        0    80209 2020-02-02 00:00:00.000000 vector-1.3.1/docs/usage/intro.ipynb
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 vector-1.3.1/docs/usage/structure.md
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/__init__.py
--rw-r--r--   0        0        0   136107 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_methods.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_typeutils.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/py.typed
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/version.pyi
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/__init__.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/Et.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/Et2.py
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/Mt.py
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/Mt2.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/__init__.py
--rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/add.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/beta.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/boostX_beta.py
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/boostX_gamma.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/boostY_beta.py
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/boostY_gamma.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/boostZ_beta.py
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/boostZ_gamma.py
--rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/boost_beta3.py
--rw-r--r--   0        0        0    21206 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/boost_p4.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/deltaRapidityPhi.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/deltaRapidityPhi2.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/dot.py
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/equal.py
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/gamma.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/is_lightlike.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/is_spacelike.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/is_timelike.py
--rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/isclose.py
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/not_equal.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/rapidity.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/scale.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/subtract.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/t.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/t2.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/tau.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/tau2.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/to_beta3.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/transform4D.py
--rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/lorentz/unit.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/__init__.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/add.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/deltaphi.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/dot.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/equal.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/is_antiparallel.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/is_parallel.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/is_perpendicular.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/isclose.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/not_equal.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/phi.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/rho.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/rho2.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/rotateZ.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/scale.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/subtract.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/transform2D.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/unit.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/x.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/planar/y.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/__init__.py
--rw-r--r--   0        0        0    15730 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/add.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/costheta.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/cottheta.py
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/cross.py
--rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/deltaR.py
--rw-r--r--   0        0        0    13511 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/deltaR2.py
--rw-r--r--   0        0        0    14836 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/deltaangle.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/deltaeta.py
--rw-r--r--   0        0        0    15430 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/dot.py
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/equal.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/eta.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/is_antiparallel.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/is_parallel.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/is_perpendicular.py
--rw-r--r--   0        0        0    16524 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/isclose.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/mag.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/mag2.py
--rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/not_equal.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/rotateX.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/rotateY.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/rotate_axis.py
--rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/rotate_euler.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/rotate_quaternion.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/scale.py
--rw-r--r--   0        0        0    15755 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/subtract.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/theta.py
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/transform3D.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/unit.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/_compute/spatial/z.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/backends/__init__.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/backends/_numba.py
--rw-r--r--   0        0        0   116103 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/backends/_numba_object.py
--rw-r--r--   0        0        0    70597 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/backends/awkward.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/backends/awkward_constructors.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/backends/numba_numpy.py
--rw-r--r--   0        0        0    70367 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/backends/numpy.py
--rw-r--r--   0        0        0   100958 2020-02-02 00:00:00.000000 vector-1.3.1/src/vector/backends/object.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 vector-1.3.1/tests/test_compute_features.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 vector-1.3.1/tests/test_issues.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 vector-1.3.1/tests/test_methods.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 vector-1.3.1/tests/test_notebooks.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.3.1/tests/backends/__init__.py
--rw-r--r--   0        0        0    28832 2020-02-02 00:00:00.000000 vector-1.3.1/tests/backends/test_awkward.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 vector-1.3.1/tests/backends/test_awkward_numba.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 vector-1.3.1/tests/backends/test_dask_awkward.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 vector-1.3.1/tests/backends/test_numba_numpy.py
--rw-r--r--   0        0        0    54479 2020-02-02 00:00:00.000000 vector-1.3.1/tests/backends/test_numba_object.py
--rw-r--r--   0        0        0    14805 2020-02-02 00:00:00.000000 vector-1.3.1/tests/backends/test_numpy.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 vector-1.3.1/tests/backends/test_object.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 vector-1.3.1/tests/backends/test_operators.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/__init__.py
--rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/test_add.py
--rw-r--r--   0        0        0    35059 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/test_conversions.py
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/test_dot.py
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/test_equal.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/test_isclose.py
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/test_not_equal.py
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/test_scale.py
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/test_subtract.py
--rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/test_unit.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/__init__.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_Et.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_Et2.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_Mt.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_Mt2.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_beta.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_boostX_beta.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_boostX_gamma.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_boostY_beta.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_boostY_gamma.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_boostZ_beta.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_boostZ_gamma.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_boost_beta3.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_boost_p4.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_deltaRapidityPhi.py
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_deltaRapidityPhi2.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_gamma.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_rapidity.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_t.py
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_t2.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_tau.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_tau2.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/lorentz/test_to_beta3.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/planar/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/planar/test_deltaphi.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/planar/test_phi.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/planar/test_rho.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/planar/test_rho2.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/planar/test_rotateZ.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/planar/test_x.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/planar/test_y.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_costheta.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_cottheta.py
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_cross.py
--rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_deltaR.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_deltaR2.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_deltaangle.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_deltaeta.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_eta.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_mag.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_mag2.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_rotateX.py
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_rotateY.py
--rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_rotate_axis.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_rotate_euler.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_rotate_quaternion.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_theta.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 vector-1.3.1/tests/compute/spatial/test_z.py
--rw-r--r--   0        0        0   235709 2020-02-02 00:00:00.000000 vector-1.3.1/tests/samples/issue-161-v2.pkl
--rw-r--r--   0        0        0   231208 2020-02-02 00:00:00.000000 vector-1.3.1/tests/samples/issue-161.pkl
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 vector-1.3.1/.gitignore
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 vector-1.3.1/LICENSE
--rw-r--r--   0        0        0    34462 2020-02-02 00:00:00.000000 vector-1.3.1/README.md
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 vector-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    37462 2020-02-02 00:00:00.000000 vector-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 vector-1.4.0/.all-contributorsrc
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 vector-1.4.0/.git_archival.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 vector-1.4.0/.gitattributes
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 vector-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 vector-1.4.0/.readthedocs.yml
+-rwxr-xr-x   0        0        0      887 2020-02-02 00:00:00.000000 vector-1.4.0/CITATION.cff
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 vector-1.4.0/environment.yml
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 vector-1.4.0/noxfile.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 vector-1.4.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 vector-1.4.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 vector-1.4.0/.github/codecov.yml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 vector-1.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 vector-1.4.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 vector-1.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 vector-1.4.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 vector-1.4.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 vector-1.4.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 vector-1.4.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 vector-1.4.0/.github/workflows/notebooks.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 vector-1.4.0/docs/Makefile
+-rw-r--r--   0        0        0    14211 2020-02-02 00:00:00.000000 vector-1.4.0/docs/changelog.md
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 vector-1.4.0/docs/conf.py
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 vector-1.4.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 vector-1.4.0/docs/make.bat
+-rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 vector-1.4.0/docs/_images/LogoSrc.svg
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 vector-1.4.0/docs/_images/vector-logo.png
+-rw-r--r--   0        0        0   174177 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/inheritance.svg
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/modules.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/vector._methods.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/vector._typeutils.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/vector.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/backends/vector.backends._numba.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/backends/vector.backends._numba_object.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/backends/vector.backends.awkward.rst
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/backends/vector.backends.awkward_constructors.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/backends/vector.backends.numba_numpy.rst
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/backends/vector.backends.numpy.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/backends/vector.backends.object.rst
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/backends/vector.backends.rst
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/vector._compute.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.Et.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.Et2.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.Mt.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.Mt2.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.add.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.beta.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.boostX_beta.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.boostX_gamma.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.boostY_beta.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.boostY_gamma.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.boostZ_beta.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.boostZ_gamma.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.boost_beta3.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.boost_p4.rst
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.deltaRapidityPhi.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.deltaRapidityPhi2.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.dot.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.equal.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.gamma.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.is_lightlike.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.is_spacelike.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.is_timelike.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.isclose.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.not_equal.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.rapidity.rst
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.scale.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.subtract.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.t.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.t2.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.tau.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.tau2.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.to_beta3.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.transform4D.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.unit.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.add.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.deltaphi.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.dot.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.equal.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.is_antiparallel.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.is_parallel.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.is_perpendicular.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.isclose.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.not_equal.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.phi.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.rho.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.rho2.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.rotateZ.rst
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.scale.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.subtract.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.transform2D.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.unit.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.x.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/planar/vector._compute.planar.y.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.add.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.costheta.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.cottheta.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.cross.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.deltaR.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.deltaR2.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.deltaangle.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.deltaeta.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.dot.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.equal.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.eta.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.is_antiparallel.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.is_parallel.rst
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.is_perpendicular.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.isclose.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.mag.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.mag2.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.not_equal.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.rotateX.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.rotateY.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.rotate_axis.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.rotate_euler.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.rotate_quaternion.rst
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.scale.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.subtract.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.theta.rst
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.transform3D.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.unit.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.z.rst
+-rw-r--r--   0        0        0   167521 2020-02-02 00:00:00.000000 vector-1.4.0/docs/usage/intro.ipynb
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 vector-1.4.0/docs/usage/structure.md
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/__init__.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_lib.py
+-rw-r--r--   0        0        0   141816 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_methods.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_typeutils.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/py.typed
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/version.pyi
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/__init__.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/Et.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/Et2.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/Mt.py
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/Mt2.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/__init__.py
+-rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/add.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/beta.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/boostX_beta.py
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/boostX_gamma.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/boostY_beta.py
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/boostY_gamma.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/boostZ_beta.py
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/boostZ_gamma.py
+-rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/boost_beta3.py
+-rw-r--r--   0        0        0    21206 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/boost_p4.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/deltaRapidityPhi.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/deltaRapidityPhi2.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/dot.py
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/equal.py
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/gamma.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/is_lightlike.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/is_spacelike.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/is_timelike.py
+-rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/isclose.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/not_equal.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/rapidity.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/scale.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/subtract.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/t.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/t2.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/tau.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/tau2.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/to_beta3.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/transform4D.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/lorentz/unit.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/add.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/deltaphi.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/dot.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/equal.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/is_antiparallel.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/is_parallel.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/is_perpendicular.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/isclose.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/not_equal.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/phi.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/rho.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/rho2.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/rotateZ.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/scale.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/subtract.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/transform2D.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/unit.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/x.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/planar/y.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/__init__.py
+-rw-r--r--   0        0        0    15730 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/add.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/costheta.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/cottheta.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/cross.py
+-rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/deltaR.py
+-rw-r--r--   0        0        0    13511 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/deltaR2.py
+-rw-r--r--   0        0        0    14836 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/deltaangle.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/deltaeta.py
+-rw-r--r--   0        0        0    15430 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/dot.py
+-rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/equal.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/eta.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/is_antiparallel.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/is_parallel.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/is_perpendicular.py
+-rw-r--r--   0        0        0    16524 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/isclose.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/mag.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/mag2.py
+-rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/not_equal.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/rotateX.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/rotateY.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/rotate_axis.py
+-rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/rotate_euler.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/rotate_quaternion.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/scale.py
+-rw-r--r--   0        0        0    15755 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/subtract.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/theta.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/transform3D.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/unit.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/_compute/spatial/z.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/backends/__init__.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/backends/_numba.py
+-rw-r--r--   0        0        0   116103 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/backends/_numba_object.py
+-rw-r--r--   0        0        0    70597 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/backends/awkward.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/backends/awkward_constructors.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/backends/numba_numpy.py
+-rw-r--r--   0        0        0    70367 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/backends/numpy.py
+-rw-r--r--   0        0        0   100966 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/backends/object.py
+-rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 vector-1.4.0/src/vector/backends/sympy.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 vector-1.4.0/tests/test_compute_features.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 vector-1.4.0/tests/test_issues.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 vector-1.4.0/tests/test_methods.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 vector-1.4.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/__init__.py
+-rw-r--r--   0        0        0    28832 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/test_awkward.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/test_awkward_numba.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/test_dask_awkward.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/test_numba_numpy.py
+-rw-r--r--   0        0        0    54479 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/test_numba_object.py
+-rw-r--r--   0        0        0    14805 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/test_numpy.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/test_object.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/test_operators.py
+-rw-r--r--   0        0        0    14861 2020-02-02 00:00:00.000000 vector-1.4.0/tests/backends/test_sympy.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/__init__.py
+-rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/test_add.py
+-rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/test_conversions.py
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/test_dot.py
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/test_equal.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/test_isclose.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/test_not_equal.py
+-rw-r--r--   0        0        0    11080 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/test_scale.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/test_subtract.py
+-rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/test_unit.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/__init__.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_Et.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_Et2.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_Mt.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_Mt2.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_beta.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_boostX_beta.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_boostX_gamma.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_boostY_beta.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_boostY_gamma.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_boostZ_beta.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_boostZ_gamma.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_boost_beta3.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_boost_p4.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_deltaRapidityPhi.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_deltaRapidityPhi2.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_gamma.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_rapidity.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_t.py
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_t2.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_tau.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_tau2.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/lorentz/test_to_beta3.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/planar/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/planar/test_deltaphi.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/planar/test_phi.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/planar/test_rho.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/planar/test_rho2.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/planar/test_rotateZ.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/planar/test_x.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/planar/test_y.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_costheta.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_cottheta.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_cross.py
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_deltaR.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_deltaR2.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_deltaangle.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_deltaeta.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_eta.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_mag.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_mag2.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_rotateX.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_rotateY.py
+-rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_rotate_axis.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_rotate_euler.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_rotate_quaternion.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_theta.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/spatial/test_z.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_add.py
+-rw-r--r--   0        0        0    20973 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_conversions.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_dot.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_equal.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_is_antiparallel.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_is_parallel.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_is_perpendicular.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_not_equal.py
+-rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_scale.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_subtract.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/test_unit.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/__init__.py
+-rw-r--r--   0        0        0     7022 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_Et.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_Et2.py
+-rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_Mt.py
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_Mt2.py
+-rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_beta.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_boostX_beta.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_boostX_gamma.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_boostY_beta.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_boostY_gamma.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_boostZ_beta.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_boostZ_gamma.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_boost_beta3.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_boost_p4.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_deltaRapidityPhi.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_deltaRapidityPhi2.py
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_gamma.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_is_lightlike.py
+-rw-r--r--   0        0        0    13705 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_is_spacelike.py
+-rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_is_timelike.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_rapidity.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_t.py
+-rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_t2.py
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_tau.py
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_tau2.py
+-rw-r--r--   0        0        0    14113 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/lorentz/test_to_beta3.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/planar/__init__.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/planar/test_deltaphi.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/planar/test_phi.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/planar/test_rho.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/planar/test_rho2.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/planar/test_rotateZ.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/planar/test_x.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/planar/test_y.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/__init__.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_costheta.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_cottheta.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_cross.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_deltaR.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_deltaR2.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_deltaangle.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_deltaeta.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_eta.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_mag.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_mag2.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_rotateX.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_rotateY.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_rotate_axis.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_rotate_euler.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_rotate_quaternion.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_theta.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 vector-1.4.0/tests/compute/sympy/spatial/test_z.py
+-rw-r--r--   0        0        0   235709 2020-02-02 00:00:00.000000 vector-1.4.0/tests/samples/issue-161-v2.pkl
+-rw-r--r--   0        0        0   231208 2020-02-02 00:00:00.000000 vector-1.4.0/tests/samples/issue-161.pkl
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 vector-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 vector-1.4.0/LICENSE
+-rw-r--r--   0        0        0    37569 2020-02-02 00:00:00.000000 vector-1.4.0/README.md
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 vector-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    40667 2020-02-02 00:00:00.000000 vector-1.4.0/PKG-INFO
```

### Comparing `vector-1.3.1/.all-contributorsrc` & `vector-1.4.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/.pre-commit-config.yaml` & `vector-1.4.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
         exclude: ^docs
       - id: mixed-line-ending
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.2"
+    rev: "v0.4.1"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: "1.7.0"
+    rev: "1.8.0"
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.9.0
     hooks:
       - id: mypy
         files: src
         args: []
         additional_dependencies:
           - numpy
           - packaging
+          - sympy
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
+        exclude: ^docs/usage/intro.ipynb$
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         exclude: assets/js/webapp\.js
@@ -65,13 +67,13 @@
       - id: python-check-blanket-type-ignore
         exclude: ^src/vector/backends/_numba_object.py$
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.8.4
+    rev: 1.8.5
     hooks:
       - id: nbqa-pyupgrade
         args: ["--py37-plus"]
       - id: nbqa-isort
         args: ["--float-to-top"]
```

### Comparing `vector-1.3.1/CITATION.cff` & `vector-1.4.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/noxfile.py` & `vector-1.4.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,29 @@
     session.install("-e", ".[test]")
     session.run("pytest", "--ignore", "tests/test_notebooks.py", *session.posargs)
 
 
 @nox.session(reuse_venv=True)
 def tests(session: nox.Session) -> None:
     """Run the unit and regular tests."""
-    session.install("-e", ".[awkward,numba,test,test-extras]")
+    session.install("-e", ".[awkward,numba,test,test-extras,sympy]")
     session.run("pytest", "--ignore", "tests/test_notebooks.py", *session.posargs)
 
 
 @nox.session(reuse_venv=True)
 def coverage(session: nox.Session) -> None:
     """Run tests and compute coverage."""
     session.posargs.append("--cov=vector")
     tests(session)
 
 
 @nox.session(reuse_venv=True)
 def doctests(session: nox.Session) -> None:
     """Run the doctests."""
-    session.install("-e", ".[awkward,numba,test,test-extras]")
+    session.install("-e", ".[awkward,numba,test,test-extras,sympy]")
     session.run("pytest", "--doctest-plus", "src/vector/", *session.posargs)
 
 
 @nox.session(reuse_venv=True)
 def notebooks(session: nox.Session) -> None:
     """Run the notebook tests"""
     session.install("-e", ".[awkward,numba,test,test-extras]", "numba")
```

### Comparing `vector-1.3.1/.github/CONTRIBUTING.md` & `vector-1.4.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/.github/PULL_REQUEST_TEMPLATE.md` & `vector-1.4.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `vector-1.4.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `vector-1.4.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/.github/matchers/pylint.json` & `vector-1.4.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/.github/workflows/cd.yml` & `vector-1.4.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/.github/workflows/ci.yml` & `vector-1.4.0/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,22 @@
 
       - name: Install package
         run: python -m pip install -e .[test]
 
       - name: Test light package
         run: python -m pytest -ra --ignore tests/test_notebooks.py
 
+      - name: Install numpy v2
+        if: matrix.python-version != 3.8
+        run: python -m pip install "numpy>=2.0.0b1"
+
+      - name: Test light package with numpy v2.x
+        if: matrix.python-version != 3.8
+        run: python -m pytest -ra --ignore tests/test_notebooks.py
+
   check-awkward-v1:
     needs: [check-light]
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version:
@@ -125,16 +133,24 @@
       - name: Run doctests on Python 3.11 with awkward v2.x
         if: matrix.python-version == 3.11
         run: python -m pytest -ra --doctest-plus src/vector/
 
       - name: Test package with awkward v2.x
         run: python -m pytest -ra --cov=vector --ignore tests/test_notebooks.py .
 
+      - name: Install numpy v2
+        if: matrix.python-version != 3.8
+        run: python -m pip install "numpy>=2.0.0b1"
+
+      - name: Test package with numpy v2.x
+        if: matrix.python-version != 3.8
+        run: python -m pytest -ra --cov=vector --ignore tests/test_notebooks.py .
+
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.3.0
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
 
   discheck:
     runs-on: ubuntu-latest
     name: Disassemble check
     steps:
```

### Comparing `vector-1.3.1/.github/workflows/notebooks.yml` & `vector-1.4.0/.github/workflows/notebooks.yml`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/Makefile` & `vector-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/changelog.md` & `vector-1.4.0/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,33 @@
 # Changelog
 
+## Version 1.4
+
+### Version 1.4.0
+
+#### Features
+
+- feat: allow coord values in to\_<coord_names> methods [#446][]
+- feat: a sympy backend [#442][]
+
+#### Bug fixes
+
+- fix: call the square implementation for power 2 on object vectors [#444][]
+- fix: use negfactor in negfactor scale test [#456][]
+
+#### Maintenance
+
+- chore: test on numpy 2.0 [#451][]
+
+[#446]: https://github.com/scikit-hep/vector/pull/446
+[#442]: https://github.com/scikit-hep/vector/pull/442
+[#444]: https://github.com/scikit-hep/vector/pull/444
+[#456]: https://github.com/scikit-hep/vector/pull/456
+[#451]: https://github.com/scikit-hep/vector/pull/451
+
 ## Version 1.3
 
 ### Version 1.3.1
 
 #### Features
 
 - feat: make momentum-ness infectious [#437][]
```

### Comparing `vector-1.3.1/docs/conf.py` & `vector-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/index.rst` & `vector-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/make.bat` & `vector-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/_images/LogoSrc.svg` & `vector-1.4.0/docs/_images/LogoSrc.svg`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/_images/vector-logo.png` & `vector-1.4.0/docs/_images/vector-logo.png`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/api/inheritance.svg` & `vector-1.4.0/docs/api/inheritance.svg`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/api/compute/lorentz/vector._compute.lorentz.rst` & `vector-1.4.0/docs/api/compute/lorentz/vector._compute.lorentz.rst`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/api/compute/planar/vector._compute.planar.rst` & `vector-1.4.0/docs/api/compute/planar/vector._compute.planar.rst`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/docs/api/compute/spatial/vector._compute.spatial.rst` & `vector-1.4.0/docs/api/compute/spatial/vector._compute.spatial.rst`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/__init__.py` & `vector-1.4.0/src/vector/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,25 +70,43 @@
 _is_awkward_v2: bool | None
 try:
     _is_awkward_v2 = packaging.version.Version(
         importlib.metadata.version("awkward")
     ) >= packaging.version.Version("2.0.0rc1")
 except importlib.metadata.PackageNotFoundError:
     _is_awkward_v2 = None
+
 try:
     import awkward
 
     _import_awkward()
 except ImportError:
     awkward = None
     if not typing.TYPE_CHECKING:
         VectorAwkward = None
 else:
     from vector.backends.awkward import VectorAwkward
 
+try:
+    import sympy
+except ImportError:
+    sympy = None  # type: ignore[assignment]
+    if not typing.TYPE_CHECKING:
+        VectorSympy = None
+else:
+    from vector.backends.sympy import (
+        MomentumSympy2D,
+        MomentumSympy3D,
+        MomentumSympy4D,
+        VectorSympy,
+        VectorSympy2D,
+        VectorSympy3D,
+        VectorSympy4D,
+    )
+
 
 __all__: tuple[str, ...] = (
     "Array",
     "Azimuthal",
     "AzimuthalRhoPhi",
     "AzimuthalXY",
     "Coordinates",
@@ -100,14 +118,17 @@
     "Momentum",
     "MomentumNumpy2D",
     "MomentumNumpy3D",
     "MomentumNumpy4D",
     "MomentumObject2D",
     "MomentumObject3D",
     "MomentumObject4D",
+    "MomentumSympy2D",
+    "MomentumSympy3D",
+    "MomentumSympy4D",
     "Planar",
     "Spatial",
     "Temporal",
     "TemporalT",
     "TemporalTau",
     "Vector",
     "Vector2D",
@@ -118,14 +139,18 @@
     "VectorNumpy2D",
     "VectorNumpy3D",
     "VectorNumpy4D",
     "VectorObject",
     "VectorObject2D",
     "VectorObject3D",
     "VectorObject4D",
+    "VectorSympy",
+    "VectorSympy2D",
+    "VectorSympy3D",
+    "VectorSympy4D",
     "__version__",
     "arr",
     "array",
     "awk",
     "zip",
     "dim",
     "obj",
```

### Comparing `vector-1.3.1/src/vector/_methods.py` & `vector-1.4.0/src/vector/_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import typing
 from contextlib import suppress
 
 import vector
 from vector._typeutils import (
     BoolCollection,
+    FloatArray,
     ScalarCollection,
     TransformProtocol2D,
     TransformProtocol3D,
     TransformProtocol4D,
 )
 
 Module = typing.Any  # returns a module, but we can't be specific about which one
@@ -271,259 +272,331 @@
         """
         raise AssertionError
 
     def to_xyz(self) -> VectorProtocolSpatial:
         """
         Converts to $x$-$y$-$z$ coordinates, possibly eliminating or imputing
         dimensions with a projection.
+
+        The $z$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_xytheta(self) -> VectorProtocolSpatial:
         r"""
         Converts to $x$-$y$-$\theta$ coordinates, possibly eliminating or imputing
         dimensions with a projection.
+
+        The $theta$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_xyeta(self) -> VectorProtocolSpatial:
         r"""
         Converts to $x$-$y$-$\eta$ coordinates, possibly eliminating or imputing
         dimensions with a projection.
+
+        The $eta$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_pxpypz(self) -> VectorProtocolSpatial:
         """
         Converts to $px$-$py$-$pz$ coordinates, possibly eliminating or imputing
         dimensions with a projection.
+
+        The $pz$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_pxpytheta(self) -> VectorProtocolSpatial:
         r"""
         Converts to $px$-$py$-$\theta$ coordinates, possibly eliminating or imputing
         dimensions with a projection.
+
+        The $theta$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_pxpyeta(self) -> VectorProtocolSpatial:
         r"""
         Converts to $px$-$py$-$\eta$ coordinates, possibly eliminating or imputing
         dimensions with a projection.
+
+        The $eta$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_rhophiz(self) -> VectorProtocolSpatial:
         r"""
         Converts to $\rho$-$\phi$-$z$ coordinates, possibly eliminating or imputing
         dimensions with a projection.
+
+        The $z$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_rhophitheta(self) -> VectorProtocolSpatial:
         r"""
         Converts to $\rho$-$\phi$-$\theta$ coordinates, possibly eliminating or
         imputing dimensions with a projection.
+
+        The $theta$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_rhophieta(self) -> VectorProtocolSpatial:
         r"""
         Converts to $\rho$-$\phi$-$\eta$ coordinates, possibly eliminating or
         imputing dimensions with a projection.
+
+        The $eta$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_ptphipz(self) -> VectorProtocolSpatial:
         r"""
         Converts to $pt$-$\phi$-$pz$ coordinates, possibly eliminating or imputing
         dimensions with a projection.
+
+        The $pz$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_ptphitheta(self) -> VectorProtocolSpatial:
         r"""
         Converts to $pt$-$\phi$-$\theta$ coordinates, possibly eliminating or
         imputing dimensions with a projection.
+
+        The $theta$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_ptphieta(self) -> VectorProtocolSpatial:
         r"""
         Converts to $pt$-$\phi$-$\eta$ coordinates, possibly eliminating or
         imputing dimensions with a projection.
+
+        The $eta$ coordinate can be passed as a named argument.
         """
         raise AssertionError
 
     def to_xyzt(self) -> VectorProtocolLorentz:
         """
         Converts to $x$-$y$-$z$-$t$ coordinates, possibly imputing dimensions with
         a projection.
+
+        The $z$ and $t$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_xyztau(self) -> VectorProtocolLorentz:
         r"""
         Converts to $x$-$y$-$z$-$\tau$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $z$ and $tau$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_xythetat(self) -> VectorProtocolLorentz:
         r"""
         Converts to $x$-$y$-$\theta$-$t$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $theta$ and $t$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_xythetatau(self) -> VectorProtocolLorentz:
         r"""
         Converts to $x$-$y$-$\theta$-$\tau$ coordinates, possibly imputing
         dimensions with a projection.
+
+        The $theta$ and $tau$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_xyetat(self) -> VectorProtocolLorentz:
         r"""
         Converts to $x$-$y$-$\eta$-$t$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $eta$ and $t$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_xyetatau(self) -> VectorProtocolLorentz:
         r"""
         Converts to $x$-$y$-$\eta$-$\tau$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $eta$ and $tau$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_pxpypzenergy(self) -> VectorProtocolLorentz:
         r"""
         Converts to $px$-$py$-$pz$-$energy$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $pz$ and $energy$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_pxpythetaenergy(self) -> VectorProtocolLorentz:
         r"""
         Converts to $px$-$py$-$\theta$-$energy$ coordinates, possibly imputing
         dimensions with a projection.
+
+        The $theta$ and $energy$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_pxpyetaenergy(self) -> VectorProtocolLorentz:
         r"""
         Converts to $px$-$py$-$\eta$-$energy$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $eta$ and $energy$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_pxpypzmass(self) -> VectorProtocolLorentz:
         r"""
         Converts to $px$-$py$-$pz$-$mass$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $pz$ and $mass$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_pxpythetamass(self) -> VectorProtocolLorentz:
         r"""
         Converts to $px$-$py$-$\theta$-$energy$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $theta$ and $mass$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_pxpyetamass(self) -> VectorProtocolLorentz:
         r"""
         Converts to $px$-$py$-$\eta$-$mass$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $eta$ and $mass$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_rhophizt(self) -> VectorProtocolLorentz:
         r"""
         Converts to $\rho$-$\phi$-$z$-$t$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $z$ and $t$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_rhophiztau(self) -> VectorProtocolLorentz:
         r"""
         Converts to $\rho$-$\phi$-$z$-$\tau$ coordinates, possibly imputing
         dimensions with a projection.
+
+        The $z$ and $tau$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_rhophithetat(self) -> VectorProtocolLorentz:
         r"""
         Converts to $\rho$-$\phi$-$\theta$-$t$ coordinates, possibly imputing
         dimensions with a projection.
+
+        The $theta$ and $t$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_rhophithetatau(self) -> VectorProtocolLorentz:
         r"""
         Converts to $\rho$-$\phi$-$\theta$-$\tau$ coordinates, possibly imputing
         dimensions with a projection.
+
+        The $theta$ and $tau$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_rhophietat(self) -> VectorProtocolLorentz:
         r"""
         Converts to $\rho$-$\phi$-$\eta$-$t$ coordinates, possibly imputing
         dimensions with a projection.
+
+        The $eta$ and $t$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_rhophietatau(self) -> VectorProtocolLorentz:
         r"""
         Converts to $\rho$-$\phi$-$\eta$-$\tau$ coordinates, possibly imputing
         dimensions with a projection.
+
+        The $eta$ and $tau$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_ptphipzenergy(self) -> VectorProtocolLorentz:
         r"""
         Converts to $pt$-$\phi$-$pz$-$energy$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $pz$ and $energy$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_ptphithetaenergy(self) -> VectorProtocolLorentz:
         r"""
         Converts to $pt$-$\phi$-$\theta$-$energy$ coordinates, possibly imputing
         dimensions with a projection.
+
+        The $theta$ and $energy$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_ptphietaenergy(self) -> VectorProtocolLorentz:
         r"""
         Converts to $pt$-$\phi$-$\eta$-$energy$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $eta$ and $energy$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_ptphipzmass(self) -> VectorProtocolLorentz:
         r"""
         Converts to $pt$-$\phi$-$pz$-$mass$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $pz$ and $mass$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_ptphithetamass(self) -> VectorProtocolLorentz:
         r"""
         Converts to $pt$-$\phi$-$\theta$-$mass$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $theta$ and $mass$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def to_ptphietamass(self) -> VectorProtocolLorentz:
         r"""
         Converts to $pt$-$\phi$-$\theta$-$mass$ coordinates, possibly imputing dimensions
         with a projection.
+
+        The $eta$ and $mass$ coordinates can be passed as a named argument.
         """
         raise AssertionError
 
     def unit(self: SameVectorType) -> SameVectorType:
         """
         Returns vector(s) normalized to unit length, which is `rho == 1` for 2D
         vectors, `mag == 1` for 3D vectors, and `tau == 1` for 4D vectors.
@@ -2684,355 +2757,407 @@
             [AzimuthalRhoPhi, None],
             1,
         )
 
     def to_ptphi(self) -> VectorProtocolPlanar:
         return self.to_rhophi()
 
-    def to_xyz(self) -> VectorProtocolSpatial:
+    def to_xyz(self, *, z: float | FloatArray = 0.0) -> VectorProtocolSpatial:
         from vector._compute import planar, spatial
 
-        lcoord = 0
+        lcoord = z
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.z.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.x.dispatch(self), planar.y.dispatch(self), lcoord),
             [AzimuthalXY, LongitudinalZ, None],
             1,
         )
 
-    def to_xytheta(self) -> VectorProtocolSpatial:
+    def to_xytheta(self, *, theta: float | FloatArray = 0.0) -> VectorProtocolSpatial:
         from vector._compute import planar, spatial
 
-        lcoord = 0
+        lcoord = theta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.theta.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.x.dispatch(self), planar.y.dispatch(self), lcoord),
             [AzimuthalXY, LongitudinalTheta, None],
             1,
         )
 
-    def to_xyeta(self) -> VectorProtocolSpatial:
+    def to_xyeta(self, *, eta: float | FloatArray = 0.0) -> VectorProtocolSpatial:
         from vector._compute import planar, spatial
 
-        lcoord = 0
+        lcoord = eta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.eta.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.x.dispatch(self), planar.y.dispatch(self), lcoord),
             [AzimuthalXY, LongitudinalEta, None],
             1,
         )
 
-    def to_pxpypz(self) -> VectorProtocolSpatial:
-        return self.to_xyz()
+    def to_pxpypz(self, *, pz: float | FloatArray = 0.0) -> VectorProtocolSpatial:
+        return self.to_xyz(z=pz)
 
-    def to_pxpytheta(self) -> VectorProtocolSpatial:
-        return self.to_xytheta()
+    def to_pxpytheta(self, *, theta: float | FloatArray = 0.0) -> VectorProtocolSpatial:
+        return self.to_xytheta(theta=theta)
 
-    def to_pxpyeta(self) -> VectorProtocolSpatial:
-        return self.to_xyeta()
+    def to_pxpyeta(self, *, eta: float | FloatArray = 0.0) -> VectorProtocolSpatial:
+        return self.to_xyeta(eta=eta)
 
-    def to_rhophiz(self) -> VectorProtocolSpatial:
+    def to_rhophiz(self, *, z: float | FloatArray = 0.0) -> VectorProtocolSpatial:
         from vector._compute import planar, spatial
 
-        lcoord = 0
+        lcoord = z
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.z.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.rho.dispatch(self), planar.phi.dispatch(self), lcoord),
             [AzimuthalRhoPhi, LongitudinalZ, None],
             1,
         )
 
-    def to_rhophitheta(self) -> VectorProtocolSpatial:
+    def to_rhophitheta(
+        self, *, theta: float | FloatArray = 0.0
+    ) -> VectorProtocolSpatial:
         from vector._compute import planar, spatial
 
-        lcoord = 0
+        lcoord = theta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.theta.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.rho.dispatch(self), planar.phi.dispatch(self), lcoord),
             [AzimuthalRhoPhi, LongitudinalTheta, None],
             1,
         )
 
-    def to_rhophieta(self) -> VectorProtocolSpatial:
+    def to_rhophieta(self, *, eta: float | FloatArray = 0.0) -> VectorProtocolSpatial:
         from vector._compute import planar, spatial
 
-        lcoord = 0
+        lcoord = eta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.eta.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.rho.dispatch(self), planar.phi.dispatch(self), lcoord),
             [AzimuthalRhoPhi, LongitudinalEta, None],
             1,
         )
 
-    def to_ptphipz(self) -> VectorProtocolSpatial:
-        return self.to_rhophiz()
+    def to_ptphipz(self, *, pz: float | FloatArray = 0.0) -> VectorProtocolSpatial:
+        return self.to_rhophiz(z=pz)
 
-    def to_ptphitheta(self) -> VectorProtocolSpatial:
-        return self.to_rhophitheta()
+    def to_ptphitheta(
+        self, *, theta: float | FloatArray = 0.0
+    ) -> VectorProtocolSpatial:
+        return self.to_rhophitheta(theta=theta)
 
-    def to_ptphieta(self) -> VectorProtocolSpatial:
-        return self.to_rhophieta()
+    def to_ptphieta(self, *, eta: float | FloatArray = 0.0) -> VectorProtocolSpatial:
+        return self.to_rhophieta(eta=eta)
 
-    def to_xyzt(self) -> VectorProtocolLorentz:
+    def to_xyzt(
+        self, *, z: float | FloatArray = 0.0, t: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = z
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.z.dispatch(self)
-        tcoord = 0
+        tcoord = t
         if isinstance(self, Vector4D):
             tcoord = lorentz.t.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.x.dispatch(self), planar.y.dispatch(self), lcoord, tcoord),
             [AzimuthalXY, LongitudinalZ, TemporalT],
             1,
         )
 
-    def to_xyztau(self) -> VectorProtocolLorentz:
+    def to_xyztau(
+        self, *, z: float | FloatArray = 0.0, tau: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = z
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.z.dispatch(self)
-        tcoord = 0
+        tcoord = tau
         if isinstance(self, Vector4D):
             tcoord = lorentz.tau.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.x.dispatch(self), planar.y.dispatch(self), lcoord, tcoord),
             [AzimuthalXY, LongitudinalZ, TemporalTau],
             1,
         )
 
-    def to_xythetat(self) -> VectorProtocolLorentz:
+    def to_xythetat(
+        self, *, theta: float | FloatArray = 0.0, t: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = theta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.theta.dispatch(self)
-        tcoord = 0
+        tcoord = t
         if isinstance(self, Vector4D):
             tcoord = lorentz.t.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.x.dispatch(self), planar.y.dispatch(self), lcoord, tcoord),
             [AzimuthalXY, LongitudinalTheta, TemporalT],
             1,
         )
 
-    def to_xythetatau(self) -> VectorProtocolLorentz:
+    def to_xythetatau(
+        self, *, theta: float | FloatArray = 0.0, tau: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = theta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.theta.dispatch(self)
-        tcoord = 0
+        tcoord = tau
         if isinstance(self, Vector4D):
             tcoord = lorentz.tau.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.x.dispatch(self), planar.y.dispatch(self), lcoord, tcoord),
             [AzimuthalXY, LongitudinalTheta, TemporalTau],
             1,
         )
 
-    def to_xyetat(self) -> VectorProtocolLorentz:
+    def to_xyetat(
+        self, *, eta: float | FloatArray = 0.0, t: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = eta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.eta.dispatch(self)
-        tcoord = 0
+        tcoord = t
         if isinstance(self, Vector4D):
             tcoord = lorentz.t.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.x.dispatch(self), planar.y.dispatch(self), lcoord, tcoord),
             [AzimuthalXY, LongitudinalEta, TemporalT],
             1,
         )
 
-    def to_xyetatau(self) -> VectorProtocolLorentz:
+    def to_xyetatau(
+        self, *, eta: float | FloatArray = 0.0, tau: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = eta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.eta.dispatch(self)
-        tcoord = 0
+        tcoord = tau
         if isinstance(self, Vector4D):
             tcoord = lorentz.tau.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.x.dispatch(self), planar.y.dispatch(self), lcoord, tcoord),
             [AzimuthalXY, LongitudinalEta, TemporalTau],
             1,
         )
 
-    def to_pxpypzenergy(self) -> VectorProtocolLorentz:
-        return self.to_xyzt()
+    def to_pxpypzenergy(
+        self, *, pz: float | FloatArray = 0.0, energy: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_xyzt(z=pz, t=energy)
 
-    def to_pxpythetaenergy(self) -> VectorProtocolLorentz:
-        return self.to_xythetat()
+    def to_pxpythetaenergy(
+        self, *, theta: float | FloatArray = 0.0, energy: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_xythetat(theta=theta, t=energy)
 
-    def to_pxpyetaenergy(self) -> VectorProtocolLorentz:
-        return self.to_xyetat()
+    def to_pxpyetaenergy(
+        self, *, eta: float | FloatArray = 0.0, energy: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_xyetat(eta=eta, t=energy)
 
-    def to_pxpypzmass(self) -> VectorProtocolLorentz:
-        return self.to_xyztau()
+    def to_pxpypzmass(
+        self, *, pz: float | FloatArray = 0.0, mass: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_xyztau(z=pz, tau=mass)
 
-    def to_pxpythetamass(self) -> VectorProtocolLorentz:
-        return self.to_xythetatau()
+    def to_pxpythetamass(
+        self, *, theta: float | FloatArray = 0.0, mass: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_xythetatau(theta=theta, tau=mass)
 
-    def to_pxpyetamass(self) -> VectorProtocolLorentz:
-        return self.to_xyetatau()
+    def to_pxpyetamass(
+        self, *, eta: float | FloatArray = 0.0, mass: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_xyetatau(eta=eta, tau=mass)
 
-    def to_rhophizt(self) -> VectorProtocolLorentz:
+    def to_rhophizt(
+        self, *, z: float | FloatArray = 0.0, t: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = z
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.z.dispatch(self)
-        tcoord = 0
+        tcoord = t
         if isinstance(self, Vector4D):
             tcoord = lorentz.t.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.rho.dispatch(self), planar.phi.dispatch(self), lcoord, tcoord),
             [AzimuthalRhoPhi, LongitudinalZ, TemporalT],
             1,
         )
 
-    def to_rhophiztau(self) -> VectorProtocolLorentz:
+    def to_rhophiztau(
+        self, *, z: float | FloatArray = 0.0, tau: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = z
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.z.dispatch(self)
-        tcoord = 0
+        tcoord = tau
         if isinstance(self, Vector4D):
             tcoord = lorentz.tau.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.rho.dispatch(self), planar.phi.dispatch(self), lcoord, tcoord),
             [AzimuthalRhoPhi, LongitudinalZ, TemporalTau],
             1,
         )
 
-    def to_rhophithetat(self) -> VectorProtocolLorentz:
+    def to_rhophithetat(
+        self, *, theta: float | FloatArray = 0.0, t: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = theta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.theta.dispatch(self)
-        tcoord = 0
+        tcoord = t
         if isinstance(self, Vector4D):
             tcoord = lorentz.t.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.rho.dispatch(self), planar.phi.dispatch(self), lcoord, tcoord),
             [AzimuthalRhoPhi, LongitudinalTheta, TemporalT],
             1,
         )
 
-    def to_rhophithetatau(self) -> VectorProtocolLorentz:
+    def to_rhophithetatau(
+        self, *, theta: float | FloatArray = 0.0, tau: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = theta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.theta.dispatch(self)
-        tcoord = 0
+        tcoord = tau
         if isinstance(self, Vector4D):
             tcoord = lorentz.tau.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.rho.dispatch(self), planar.phi.dispatch(self), lcoord, tcoord),
             [AzimuthalRhoPhi, LongitudinalTheta, TemporalTau],
             1,
         )
 
-    def to_rhophietat(self) -> VectorProtocolLorentz:
+    def to_rhophietat(
+        self, *, eta: float | FloatArray = 0.0, t: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = eta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.eta.dispatch(self)
-        tcoord = 0
+        tcoord = t
         if isinstance(self, Vector4D):
             tcoord = lorentz.t.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.rho.dispatch(self), planar.phi.dispatch(self), lcoord, tcoord),
             [AzimuthalRhoPhi, LongitudinalEta, TemporalT],
             1,
         )
 
-    def to_rhophietatau(self) -> VectorProtocolLorentz:
+    def to_rhophietatau(
+        self, *, eta: float | FloatArray = 0.0, tau: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
         from vector._compute import lorentz, planar, spatial
 
-        lcoord = 0
+        lcoord = eta
         if isinstance(self, (Vector3D, Vector4D)):
             lcoord = spatial.eta.dispatch(self)
-        tcoord = 0
+        tcoord = tau
         if isinstance(self, Vector4D):
             tcoord = lorentz.tau.dispatch(self)
 
         return self._wrap_result(
             type(self),
             (planar.rho.dispatch(self), planar.phi.dispatch(self), lcoord, tcoord),
             [AzimuthalRhoPhi, LongitudinalEta, TemporalTau],
             1,
         )
 
-    def to_ptphipzenergy(self) -> VectorProtocolLorentz:
-        return self.to_rhophizt()
+    def to_ptphipzenergy(
+        self, *, pz: float | FloatArray = 0.0, energy: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_rhophizt(z=pz, t=energy)
 
-    def to_ptphithetaenergy(self) -> VectorProtocolLorentz:
-        return self.to_rhophithetat()
+    def to_ptphithetaenergy(
+        self, *, theta: float | FloatArray = 0.0, energy: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_rhophithetat(theta=theta, t=energy)
 
-    def to_ptphietaenergy(self) -> VectorProtocolLorentz:
-        return self.to_rhophietat()
+    def to_ptphietaenergy(
+        self, *, eta: float | FloatArray = 0.0, energy: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_rhophietat(eta=eta, t=energy)
 
-    def to_ptphipzmass(self) -> VectorProtocolLorentz:
-        return self.to_rhophiztau()
+    def to_ptphipzmass(
+        self, *, pz: float | FloatArray = 0.0, mass: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_rhophiztau(z=pz, tau=mass)
 
-    def to_ptphithetamass(self) -> VectorProtocolLorentz:
-        return self.to_rhophithetatau()
+    def to_ptphithetamass(
+        self, *, theta: float | FloatArray = 0.0, mass: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_rhophithetatau(theta=theta, tau=mass)
 
-    def to_ptphietamass(self) -> VectorProtocolLorentz:
-        return self.to_rhophietatau()
+    def to_ptphietamass(
+        self, *, eta: float | FloatArray = 0.0, mass: float | FloatArray = 0.0
+    ) -> VectorProtocolLorentz:
+        return self.to_rhophietatau(eta=eta, tau=mass)
 
     def like(self, other: VectorProtocol) -> VectorProtocol:
         if isinstance(other, Vector2D):
             return self.to_Vector2D()
         elif isinstance(other, Vector3D):
             return self.to_Vector3D()
         else:
@@ -3042,18 +3167,18 @@
 class Vector2D(Vector, VectorProtocolPlanar):
     def to_Vector2D(self) -> VectorProtocolPlanar:
         return self
 
     def to_Vector3D(
         self,
         *,
-        z: float | None = None,
-        pz: float | None = None,
-        theta: float | None = None,
-        eta: float | None = None,
+        z: float | FloatArray | None = None,
+        pz: float | FloatArray | None = None,
+        theta: float | FloatArray | None = None,
+        eta: float | FloatArray | None = None,
     ) -> VectorProtocolSpatial:
         """
         Converts a 2D vector to 3D vector.
 
         The scalar longitudinal coordinate is broadcasted for NumPy and Awkward
         vectors. Only a single longitudinal coordinate should be provided.
 
@@ -3067,15 +3192,15 @@
             MomentumObject3D(px=1, py=2, pz=4)
         """
         if sum(x is not None for x in (z, pz, theta, eta)) > 1:
             raise TypeError(
                 "At most one longitudinal coordinate (`z`/`pz`, `theta`, or `eta`) may be assigned (non-None)"
             )
 
-        l_value = 0.0
+        l_value: float | FloatArray = 0.0
         l_type: type[Longitudinal] = LongitudinalZ
         if any(coord is not None for coord in (z, pz)):
             l_value = next(coord for coord in (z, pz) if coord is not None)
         elif eta is not None:
             l_value = eta
             l_type = LongitudinalEta
         elif theta is not None:
@@ -3088,26 +3213,26 @@
             [_aztype(self), l_type, None],
             1,
         )
 
     def to_Vector4D(
         self,
         *,
-        z: float | None = None,
-        pz: float | None = None,
-        theta: float | None = None,
-        eta: float | None = None,
-        t: float | None = None,
-        e: float | None = None,
-        E: float | None = None,
-        energy: float | None = None,
-        tau: float | None = None,
-        m: float | None = None,
-        M: float | None = None,
-        mass: float | None = None,
+        z: float | FloatArray | None = None,
+        pz: float | FloatArray | None = None,
+        theta: float | FloatArray | None = None,
+        eta: float | FloatArray | None = None,
+        t: float | FloatArray | None = None,
+        e: float | FloatArray | None = None,
+        E: float | FloatArray | None = None,
+        energy: float | FloatArray | None = None,
+        tau: float | FloatArray | None = None,
+        m: float | FloatArray | None = None,
+        M: float | FloatArray | None = None,
+        mass: float | FloatArray | None = None,
     ) -> VectorProtocolLorentz:
         """
         Converts a 2D vector to 4D vector.
 
         The scalar longitudinal and temporal coordinates are broadcasted for NumPy and
         Awkward vectors. Only a single longitudinal and temporal coordinate should be
         provided.
@@ -3126,23 +3251,23 @@
                 "At most one longitudinal coordinate (`z`/`pz`, `theta`, or `eta`) may be assigned (non-None)"
             )
         elif sum(x is not None for x in (t, tau, m, M, mass, e, E, energy)) > 1:
             raise TypeError(
                 "At most one longitudinal coordinate (`t`/`e`/`E`/`energy`, `tau`/`m`/`M`/`mass`) may be assigned (non-None)"
             )
 
-        t_value = 0.0
+        t_value: float | FloatArray = 0.0
         t_type: type[Temporal] = TemporalT
         if any(coord is not None for coord in (tau, m, M, mass)):
             t_type = TemporalTau
             t_value = next(coord for coord in (tau, m, M, mass) if coord is not None)
         elif any(coord is not None for coord in (t, e, E, energy)):
             t_value = next(coord for coord in (t, e, E, energy) if coord is not None)
 
-        l_value = 0.0
+        l_value: float | FloatArray = 0.0
         l_type: type[Longitudinal] = LongitudinalZ
         if any(coord is not None for coord in (z, pz)):
             l_value = next(coord for coord in (z, pz) if coord is not None)
         elif eta is not None:
             l_value = eta
             l_type = LongitudinalEta
         elif theta is not None:
@@ -3186,22 +3311,22 @@
 
     def to_Vector3D(self) -> VectorProtocolSpatial:
         return self
 
     def to_Vector4D(
         self,
         *,
-        t: float | None = None,
-        e: float | None = None,
-        E: float | None = None,
-        energy: float | None = None,
-        tau: float | None = None,
-        m: float | None = None,
-        M: float | None = None,
-        mass: float | None = None,
+        t: float | FloatArray | None = None,
+        e: float | FloatArray | None = None,
+        E: float | FloatArray | None = None,
+        energy: float | FloatArray | None = None,
+        tau: float | FloatArray | None = None,
+        m: float | FloatArray | None = None,
+        M: float | FloatArray | None = None,
+        mass: float | FloatArray | None = None,
     ) -> VectorProtocolLorentz:
         """
         Converts a 3D vector to 4D vector.
 
         The scalar temporal coordinate are broadcasted for NumPy and Awkward vectors.
         Only a single temporal coordinate should be provided.
 
@@ -3215,15 +3340,15 @@
             MomentumObject4D(px=1, py=2, pz=3, mass=4)
         """
         if sum(x is not None for x in (t, tau, m, M, mass, e, E, energy)) > 1:
             raise TypeError(
                 "At most one longitudinal coordinate (`t`/`e`/`E`/`energy`, `tau`/`m`/`M`/`mass`) may be assigned (non-None)"
             )
 
-        t_value = 0.0
+        t_value: float | FloatArray = 0.0
         t_type: type[Temporal] = TemporalT
         if any(coord is not None for coord in (tau, m, M, mass)):
             t_type = TemporalTau
             t_value = next(coord for coord in (tau, m, M, mass) if coord is not None)
         elif any(coord is not None for coord in (t, e, E, energy)):
             t_value = next(coord for coord in (t, e, E, energy) if coord is not None)
 
@@ -4295,14 +4420,15 @@
         )
     return result
 
 
 _handler_priority = [
     "vector.backends.object",
     "vector.backends.numpy",
+    "vector.backends.sympy",
     "vector.backends.awkward",
 ]
 
 
 def _get_handler_index(obj: VectorProtocol) -> int:
     """Returns the index of the first valid handler checking the list of parent classes"""
     for cls in type(obj).__mro__:
```

### Comparing `vector-1.3.1/src/vector/_typeutils.py` & `vector-1.4.0/src/vector/_typeutils.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/Et.py` & `vector-1.4.0/src/vector/_compute/lorentz/Et.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/Et2.py` & `vector-1.4.0/src/vector/_compute/lorentz/Et2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/Mt.py` & `vector-1.4.0/src/vector/_compute/lorentz/Mt.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/Mt2.py` & `vector-1.4.0/src/vector/_compute/lorentz/Mt2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/__init__.py` & `vector-1.4.0/src/vector/_compute/lorentz/__init__.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/add.py` & `vector-1.4.0/src/vector/_compute/lorentz/add.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/beta.py` & `vector-1.4.0/src/vector/_compute/lorentz/beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/boostX_beta.py` & `vector-1.4.0/src/vector/_compute/lorentz/boostX_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/boostX_gamma.py` & `vector-1.4.0/src/vector/_compute/lorentz/boostX_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/boostY_beta.py` & `vector-1.4.0/src/vector/_compute/lorentz/boostY_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/boostY_gamma.py` & `vector-1.4.0/src/vector/_compute/lorentz/boostY_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/boostZ_beta.py` & `vector-1.4.0/src/vector/_compute/lorentz/boostZ_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/boostZ_gamma.py` & `vector-1.4.0/src/vector/_compute/lorentz/boostZ_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/boost_beta3.py` & `vector-1.4.0/src/vector/_compute/lorentz/boost_beta3.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/boost_p4.py` & `vector-1.4.0/src/vector/_compute/lorentz/boost_p4.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/deltaRapidityPhi.py` & `vector-1.4.0/src/vector/_compute/lorentz/deltaRapidityPhi.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/deltaRapidityPhi2.py` & `vector-1.4.0/src/vector/_compute/lorentz/deltaRapidityPhi2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/dot.py` & `vector-1.4.0/src/vector/_compute/lorentz/dot.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/equal.py` & `vector-1.4.0/src/vector/_compute/lorentz/equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/gamma.py` & `vector-1.4.0/src/vector/_compute/lorentz/gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/is_lightlike.py` & `vector-1.4.0/src/vector/_compute/lorentz/is_lightlike.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/is_spacelike.py` & `vector-1.4.0/src/vector/_compute/lorentz/is_spacelike.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/is_timelike.py` & `vector-1.4.0/src/vector/_compute/lorentz/is_timelike.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/isclose.py` & `vector-1.4.0/src/vector/_compute/lorentz/isclose.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/not_equal.py` & `vector-1.4.0/src/vector/_compute/lorentz/not_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/rapidity.py` & `vector-1.4.0/src/vector/_compute/lorentz/rapidity.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/scale.py` & `vector-1.4.0/src/vector/_compute/lorentz/scale.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/subtract.py` & `vector-1.4.0/src/vector/_compute/lorentz/subtract.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/t.py` & `vector-1.4.0/src/vector/_compute/lorentz/t.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/t2.py` & `vector-1.4.0/src/vector/_compute/lorentz/t2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/tau.py` & `vector-1.4.0/src/vector/_compute/lorentz/tau.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/tau2.py` & `vector-1.4.0/src/vector/_compute/lorentz/tau2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/to_beta3.py` & `vector-1.4.0/src/vector/_compute/lorentz/to_beta3.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/transform4D.py` & `vector-1.4.0/src/vector/_compute/lorentz/transform4D.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/lorentz/unit.py` & `vector-1.4.0/src/vector/_compute/lorentz/unit.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/__init__.py` & `vector-1.4.0/src/vector/_compute/planar/__init__.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/add.py` & `vector-1.4.0/src/vector/_compute/planar/add.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/deltaphi.py` & `vector-1.4.0/src/vector/_compute/planar/deltaphi.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/dot.py` & `vector-1.4.0/src/vector/_compute/planar/dot.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/equal.py` & `vector-1.4.0/src/vector/_compute/planar/equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/is_antiparallel.py` & `vector-1.4.0/src/vector/_compute/planar/is_antiparallel.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/is_parallel.py` & `vector-1.4.0/src/vector/_compute/planar/is_parallel.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/is_perpendicular.py` & `vector-1.4.0/src/vector/_compute/planar/is_perpendicular.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/isclose.py` & `vector-1.4.0/src/vector/_compute/planar/isclose.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/not_equal.py` & `vector-1.4.0/src/vector/_compute/planar/not_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/phi.py` & `vector-1.4.0/src/vector/_compute/planar/phi.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/rho.py` & `vector-1.4.0/src/vector/_compute/planar/rho.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/rho2.py` & `vector-1.4.0/src/vector/_compute/planar/rho2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/rotateZ.py` & `vector-1.4.0/src/vector/_compute/planar/rotateZ.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,9 +44,12 @@
 }
 
 
 def dispatch(angle: typing.Any, v: typing.Any) -> typing.Any:
     function, *returns = _from_signature(__name__, dispatch_map, (_aztype(v),))
     with numpy.errstate(all="ignore"):
         return v._wrap_result(
-            _flavor_of(v), function(v.lib, angle, *v.azimuthal.elements), returns, 1
+            _flavor_of(v),
+            function(v.lib, angle, *v.azimuthal.elements),
+            returns,
+            1,
         )
```

### Comparing `vector-1.3.1/src/vector/_compute/planar/scale.py` & `vector-1.4.0/src/vector/_compute/planar/scale.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,9 +45,12 @@
 }
 
 
 def dispatch(factor: typing.Any, v: typing.Any) -> typing.Any:
     function, *returns = _from_signature(__name__, dispatch_map, (_aztype(v),))
     with numpy.errstate(all="ignore"):
         return v._wrap_result(
-            _flavor_of(v), function(v.lib, factor, *v.azimuthal.elements), returns, 1
+            _flavor_of(v),
+            function(v.lib, factor, *v.azimuthal.elements),
+            returns,
+            1,
         )
```

### Comparing `vector-1.3.1/src/vector/_compute/planar/subtract.py` & `vector-1.4.0/src/vector/_compute/planar/subtract.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/transform2D.py` & `vector-1.4.0/src/vector/_compute/planar/transform2D.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/unit.py` & `vector-1.4.0/src/vector/_compute/planar/unit.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/x.py` & `vector-1.4.0/src/vector/_compute/planar/x.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/planar/y.py` & `vector-1.4.0/src/vector/_compute/planar/y.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/__init__.py` & `vector-1.4.0/src/vector/_compute/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/add.py` & `vector-1.4.0/src/vector/_compute/spatial/add.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/costheta.py` & `vector-1.4.0/src/vector/_compute/spatial/costheta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/cottheta.py` & `vector-1.4.0/src/vector/_compute/spatial/cottheta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/cross.py` & `vector-1.4.0/src/vector/_compute/spatial/cross.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/deltaR.py` & `vector-1.4.0/src/vector/_compute/spatial/deltaR.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/deltaR2.py` & `vector-1.4.0/src/vector/_compute/spatial/deltaR2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/deltaangle.py` & `vector-1.4.0/src/vector/_compute/spatial/deltaangle.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/deltaeta.py` & `vector-1.4.0/src/vector/_compute/spatial/deltaeta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/dot.py` & `vector-1.4.0/src/vector/_compute/spatial/dot.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/equal.py` & `vector-1.4.0/src/vector/_compute/spatial/equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/eta.py` & `vector-1.4.0/src/vector/_compute/spatial/eta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/is_antiparallel.py` & `vector-1.4.0/src/vector/_compute/spatial/is_antiparallel.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/is_parallel.py` & `vector-1.4.0/src/vector/_compute/spatial/is_parallel.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/is_perpendicular.py` & `vector-1.4.0/src/vector/_compute/spatial/is_perpendicular.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/isclose.py` & `vector-1.4.0/src/vector/_compute/spatial/isclose.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/mag.py` & `vector-1.4.0/src/vector/_compute/spatial/mag.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/mag2.py` & `vector-1.4.0/src/vector/_compute/spatial/mag2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/not_equal.py` & `vector-1.4.0/src/vector/_compute/spatial/not_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/rotateX.py` & `vector-1.4.0/src/vector/_compute/spatial/rotateX.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/rotateY.py` & `vector-1.4.0/src/vector/_compute/spatial/rotateY.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/rotate_axis.py` & `vector-1.4.0/src/vector/_compute/spatial/rotate_axis.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/rotate_euler.py` & `vector-1.4.0/src/vector/_compute/spatial/rotate_euler.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,12 +288,17 @@
             order,
         ),
     )
     with numpy.errstate(all="ignore"):
         return v._wrap_result(
             _flavor_of(v),
             function(
-                v.lib, phi, theta, psi, *v.azimuthal.elements, *v.longitudinal.elements
+                v.lib,
+                phi,
+                theta,
+                psi,
+                *v.azimuthal.elements,
+                *v.longitudinal.elements,
             ),
             returns,
             1,
         )
```

### Comparing `vector-1.3.1/src/vector/_compute/spatial/rotate_quaternion.py` & `vector-1.4.0/src/vector/_compute/spatial/rotate_quaternion.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/scale.py` & `vector-1.4.0/src/vector/_compute/spatial/scale.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/subtract.py` & `vector-1.4.0/src/vector/_compute/spatial/subtract.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/theta.py` & `vector-1.4.0/src/vector/_compute/spatial/theta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/transform3D.py` & `vector-1.4.0/src/vector/_compute/spatial/transform3D.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/unit.py` & `vector-1.4.0/src/vector/_compute/spatial/unit.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/_compute/spatial/z.py` & `vector-1.4.0/src/vector/_compute/spatial/z.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/backends/__init__.py` & `vector-1.4.0/src/vector/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/backends/_numba.py` & `vector-1.4.0/src/vector/backends/_numba.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/backends/_numba_object.py` & `vector-1.4.0/src/vector/backends/_numba_object.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/backends/awkward.py` & `vector-1.4.0/src/vector/backends/awkward.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/backends/awkward_constructors.py` & `vector-1.4.0/src/vector/backends/awkward_constructors.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/backends/numpy.py` & `vector-1.4.0/src/vector/backends/numpy.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/src/vector/backends/object.py` & `vector-1.4.0/src/vector/backends/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,16 +206,14 @@
 
 class LongitudinalObjectEta(LongitudinalObject, LongitudinalEta, TupleEta):
     """
     Class for the ``eta`` (longitudinal) coordinate of Object backend.
     Use the ``elements`` property to retrieve the coordinates.
     """
 
-    eta: float
-
     @property
     def elements(self) -> tuple[float]:
         """
         Longitudinal coordinates (``theta``) as a tuple.
         Each coordinate is a scalar and not a vector.
 
         Examples:
@@ -236,16 +234,14 @@
 
 class TemporalObjectT(TemporalObject, TemporalT, TupleT):
     """
     Class for the ``t`` (temporal) coordinate of Object backend.
     Use the ``elements`` property to retrieve the coordinates.
     """
 
-    t: float
-
     @property
     def elements(self) -> tuple[float]:
         """
         Temporal coordinates (``t``) as a tuple.
         Each coordinate is a scalar and not a vector.
 
         Examples:
@@ -383,15 +379,15 @@
     def __rtruediv__(self, other: float) -> VectorProtocol:
         return numpy.true_divide(other, self)  # type: ignore[call-overload]
 
     def __itruediv__(self: SameVectorType, other: float) -> VectorProtocol:
         return _replace_data(self, numpy.true_divide(self, other))  # type: ignore[call-overload]
 
     def __pow__(self, other: float) -> float:
-        return numpy.power(self, other)  # type: ignore[call-overload]
+        return numpy.square(self) if other == 2 else numpy.power(self, other)  # type: ignore[call-overload]
 
     def __matmul__(self, other: VectorProtocol) -> float:
         return numpy.matmul(self, other)  # type: ignore[call-overload]
 
     def __array_ufunc__(
         self,
         ufunc: typing.Any,
```

### Comparing `vector-1.3.1/tests/test_compute_features.py` & `vector-1.4.0/tests/test_compute_features.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/test_issues.py` & `vector-1.4.0/tests/test_issues.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # or https://github.com/scikit-hep/vector for details.
 
 from __future__ import annotations
 
 import os
 import pickle
 
+import numpy as np
 import pytest
 
 import vector
 
 
 def test_issue_99():
     ak = pytest.importorskip("awkward")
@@ -43,7 +44,20 @@
         if not vector._is_awkward_v2
         else os.path.join("tests", "samples", "issue-161-v2.pkl")
     )
 
     with open(file_path, "rb") as f:
         a = ak.from_buffers(*pickle.load(f))
     repro(generator_like_jet_constituents=a.constituents)
+
+
+def test_issue_443():
+    ak = pytest.importorskip("awkward")
+    vector.register_awkward()
+
+    assert vector.array({"E": [1], "px": [1], "py": [1], "pz": [1]}) ** 2 == np.array(
+        [-2.0]
+    )
+    assert ak.zip(
+        {"E": [1], "px": [1], "py": [1], "pz": [1]}, with_name="Momentum4D"
+    ) ** 2 == ak.Array([-2])
+    assert vector.obj(E=1, px=1, py=1, pz=1) ** 2 == -2
```

### Comparing `vector-1.3.1/tests/test_methods.py` & `vector-1.4.0/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/backends/test_awkward.py` & `vector-1.4.0/tests/backends/test_awkward.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/backends/test_awkward_numba.py` & `vector-1.4.0/tests/backends/test_awkward_numba.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/backends/test_dask_awkward.py` & `vector-1.4.0/tests/backends/test_dask_awkward.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/backends/test_numba_numpy.py` & `vector-1.4.0/tests/backends/test_numba_numpy.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/backends/test_numba_object.py` & `vector-1.4.0/tests/backends/test_numba_object.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/backends/test_numpy.py` & `vector-1.4.0/tests/backends/test_numpy.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/backends/test_object.py` & `vector-1.4.0/tests/backends/test_object.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/backends/test_operators.py` & `vector-1.4.0/tests/backends/test_operators.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/test_add.py` & `vector-1.4.0/tests/compute/test_add.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,14 @@
     out = v1.add(v2)
     assert out.x == pytest.approx(8)
     assert out.y == pytest.approx(16)
     assert out.z == pytest.approx(6)
 
     for t1 in "xyz", "xytheta", "xyeta", "rhophiz", "rhophitheta", "rhophieta":
         for t2 in "xyz", "xytheta", "xyeta", "rhophiz", "rhophitheta", "rhophieta":
-            print(t1, t2)
-
             transformed1, transformed2 = (
                 getattr(v1, "to_" + t1)(),
                 getattr(v2, "to_" + t2)(),
             )
             out = transformed1.add(transformed2)
             assert out.x == pytest.approx(8)
             assert out.y == pytest.approx(16)
```

### Comparing `vector-1.3.1/tests/compute/test_conversions.py` & `vector-1.4.0/tests/compute/test_conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -680,34 +680,14 @@
     assert v3 + v2.like(v3) == vector.obj(px=11, py=22, pz=33, E=40)
     assert v2.like(v3) + v3 == vector.obj(px=11, py=22, pz=33, E=40)
 
     v1 = vector.obj(px=0.1, py=0.2)
     v2 = vector.obj(x=1, y=2, z=3)
     v3 = vector.obj(px=10, py=20, pz=30, t=40)
 
-    # momentum + generic = generic
-    # 2D + 3D.like(2D) = 2D
-    assert v1 + v2.like(v1) == vector.obj(x=1.1, y=2.2)
-    assert v2.like(v1) + v1 == vector.obj(x=1.1, y=2.2)
-    # 2D + 4D.like(2D) = 2D
-    assert v1 + v3.like(v1) == vector.obj(x=10.1, y=20.2)
-    assert v3.like(v1) + v1 == vector.obj(x=10.1, y=20.2)
-    # 3D + 2D.like(3D) = 3D
-    assert v2 + v1.like(v2) == vector.obj(x=1.1, y=2.2, z=3)
-    assert v1.like(v2) + v2 == vector.obj(x=1.1, y=2.2, z=3)
-    # 3D + 4D.like(3D) = 3D
-    assert v2 + v3.like(v2) == vector.obj(x=11, y=22, z=33)
-    assert v3.like(v2) + v2 == vector.obj(x=11, y=22, z=33)
-    # 4D + 2D.like(4D) = 4D
-    assert v3 + v1.like(v3) == vector.obj(x=10.1, y=20.2, z=30.0, t=40.0)
-    assert v1.like(v3) + v3 == vector.obj(x=10.1, y=20.2, z=30.0, t=40.0)
-    # 4D + 3D.like(4D) = 4D
-    assert v3 + v2.like(v3) == vector.obj(x=11, y=22, z=33, t=40)
-    assert v2.like(v3) + v3 == vector.obj(x=11, y=22, z=33, t=40)
-
 
 def test_like_numpy():
     v1 = vector.array(
         {
             "x": [10.0, 20.0, 30.0],
             "y": [-10.0, 20.0, 30.0],
         },
@@ -859,15 +839,15 @@
     assert all(v3 + v1.like(v3) == pv1_v3)
     assert all(v1.like(v3) + v3 == pv1_v3)
     # 4D + 3D.like(4D) = 4D
     assert all(v3 + v2.like(v3) == pv3_v2)
     assert all(v2.like(v3) + v3 == pv3_v2)
 
 
-def test_momentum_preservation():
+def test_momentum_preservation_object():
     v1 = vector.obj(px=0.1, py=0.2)
     v2 = vector.obj(x=1, y=2, z=3)
     v3 = vector.obj(px=10, py=20, pz=30, t=40)
 
     # momentum + generic = momentum
     # 2D + 3D.like(2D) = 2D
     assert isinstance(v1 + v2.like(v1), vector.MomentumObject2D)
@@ -885,15 +865,15 @@
     assert isinstance(v3 + v1.like(v3), vector.MomentumObject4D)
     assert isinstance(v1.like(v3) + v3, vector.MomentumObject4D)
     # 4D + 3D.like(4D) = 4D
     assert isinstance(v3 + v2.like(v3), vector.MomentumObject4D)
     assert isinstance(v2.like(v3) + v3, vector.MomentumObject4D)
 
 
-def test_flavor_of_numpy():
+def test_momentum_preservation_numpy():
     v1 = vector.array(
         {
             "px": [10.0, 20.0, 30.0],
             "py": [-10.0, 20.0, 30.0],
         },
     )
     v2 = vector.array(
```

### Comparing `vector-1.3.1/tests/compute/test_dot.py` & `vector-1.4.0/tests/compute/test_dot.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/test_equal.py` & `vector-1.4.0/tests/compute/test_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/test_isclose.py` & `vector-1.4.0/tests/compute/test_isclose.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,14 @@
         azimuthal=vector.backends.object.AzimuthalObjectXY(0.1, 0.2),
         longitudinal=vector.backends.object.LongitudinalObjectZ(0.3),
     )
     assert v1.isclose(v2)
 
     for t1 in "xyz", "xytheta", "xyeta", "rhophiz", "rhophitheta", "rhophieta":
         for t2 in "xyz", "xytheta", "xyeta", "rhophiz", "rhophitheta", "rhophieta":
-            print(t1, t2)
-
             transformed1, transformed2 = (
                 getattr(v1, "to_" + t1)(),
                 getattr(v2, "to_" + t2)(),
             )
             assert transformed1.isclose(transformed2)
```

### Comparing `vector-1.3.1/tests/compute/test_not_equal.py` & `vector-1.4.0/tests/compute/test_not_equal.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/test_scale.py` & `vector-1.4.0/tests/compute/test_scale.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,22 +267,22 @@
         "xythetat",
         "xyetat",
         "rhophizt",
         "rhophithetat",
         "rhophietat",
     ):
         tvec = getattr(vec, "to_" + t1)()
-        out = tvec.scale(1.75)
+        out = tvec.scale(-1.75)
         assert type(out.azimuthal) == type(tvec.azimuthal)  # noqa: E721
         assert type(out.longitudinal) == type(tvec.longitudinal)  # noqa: E721
         assert type(out.temporal) == type(tvec.temporal)  # noqa: E721
-        assert out.x == pytest.approx(1 * 1.75)
-        assert out.y == pytest.approx(2 * 1.75)
-        assert out.z == pytest.approx(3 * 1.75)
-        assert out.t == pytest.approx(-1.5 * 1.75)
+        assert out.x == pytest.approx(1 * -1.75)
+        assert out.y == pytest.approx(2 * -1.75)
+        assert out.z == pytest.approx(3 * -1.75)
+        assert out.t == pytest.approx(-1.5 * -1.75)
 
     for t1 in (
         "xyztau",
         "xythetatau",
         "xyetatau",
         "rhophiztau",
         "rhophithetatau",
```

### Comparing `vector-1.3.1/tests/compute/test_subtract.py` & `vector-1.4.0/tests/compute/test_subtract.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/test_unit.py` & `vector-1.4.0/tests/compute/test_unit.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_Et.py` & `vector-1.4.0/tests/compute/lorentz/test_Et.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_Et2.py` & `vector-1.4.0/tests/compute/lorentz/test_Et2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_Mt.py` & `vector-1.4.0/tests/compute/lorentz/test_Mt.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_Mt2.py` & `vector-1.4.0/tests/compute/lorentz/test_Mt2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_beta.py` & `vector-1.4.0/tests/compute/lorentz/test_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_boostX_beta.py` & `vector-1.4.0/tests/compute/lorentz/test_boostX_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_boostX_gamma.py` & `vector-1.4.0/tests/compute/lorentz/test_boostX_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_boostY_beta.py` & `vector-1.4.0/tests/compute/lorentz/test_boostY_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_boostY_gamma.py` & `vector-1.4.0/tests/compute/lorentz/test_boostY_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_boostZ_beta.py` & `vector-1.4.0/tests/compute/lorentz/test_boostZ_beta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_boostZ_gamma.py` & `vector-1.4.0/tests/compute/lorentz/test_boostZ_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_boost_beta3.py` & `vector-1.4.0/tests/compute/lorentz/test_boost_beta3.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_boost_p4.py` & `vector-1.4.0/tests/compute/lorentz/test_boost_p4.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_deltaRapidityPhi.py` & `vector-1.4.0/tests/compute/lorentz/test_deltaRapidityPhi.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_deltaRapidityPhi2.py` & `vector-1.4.0/tests/compute/lorentz/test_deltaRapidityPhi2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_gamma.py` & `vector-1.4.0/tests/compute/lorentz/test_gamma.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_rapidity.py` & `vector-1.4.0/tests/compute/lorentz/test_rapidity.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_t.py` & `vector-1.4.0/tests/compute/lorentz/test_t.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_t2.py` & `vector-1.4.0/tests/compute/lorentz/test_t2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_tau.py` & `vector-1.4.0/tests/compute/lorentz/test_tau.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_tau2.py` & `vector-1.4.0/tests/compute/lorentz/test_tau2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/lorentz/test_to_beta3.py` & `vector-1.4.0/tests/compute/lorentz/test_to_beta3.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/planar/test_deltaphi.py` & `vector-1.4.0/tests/compute/planar/test_deltaphi.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/planar/test_phi.py` & `vector-1.4.0/tests/compute/planar/test_phi.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/planar/test_rho.py` & `vector-1.4.0/tests/compute/planar/test_rho.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/planar/test_rho2.py` & `vector-1.4.0/tests/compute/planar/test_rho2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/planar/test_rotateZ.py` & `vector-1.4.0/tests/compute/planar/test_rotateZ.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/planar/test_x.py` & `vector-1.4.0/tests/compute/planar/test_x.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/planar/test_y.py` & `vector-1.4.0/tests/compute/planar/test_y.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_costheta.py` & `vector-1.4.0/tests/compute/spatial/test_costheta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_cottheta.py` & `vector-1.4.0/tests/compute/spatial/test_cottheta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_cross.py` & `vector-1.4.0/tests/compute/spatial/test_rotate_axis.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,162 +9,193 @@
 import pytest
 
 import vector.backends.numpy
 import vector.backends.object
 
 
 def test_spatial_object():
-    v1 = vector.backends.object.VectorObject3D(
+    axis = vector.backends.object.VectorObject3D(
         azimuthal=vector.backends.object.AzimuthalObjectXY(0.1, 0.2),
         longitudinal=vector.backends.object.LongitudinalObjectZ(0.3),
     )
-    v2 = vector.backends.object.VectorObject3D(
+    vec = vector.backends.object.VectorObject3D(
         azimuthal=vector.backends.object.AzimuthalObjectXY(0.4, 0.5),
         longitudinal=vector.backends.object.LongitudinalObjectZ(0.6),
     )
-    out = v1.cross(v2)
+    out = vec.rotate_axis(axis, 0.25)
     assert isinstance(out, vector.backends.object.VectorObject3D)
     assert isinstance(out.azimuthal, vector.backends.object.AzimuthalObjectXY)
     assert isinstance(out.longitudinal, vector.backends.object.LongitudinalObjectZ)
-    assert (out.x, out.y, out.z) == pytest.approx((-0.03, 0.06, -0.03))
+    assert out.x == pytest.approx(0.37483425404335763)
+    assert out.y == pytest.approx(0.5383405688588193)
+    assert out.z == pytest.approx(0.5828282027463345)
 
     for t1 in "xyz", "xytheta", "xyeta", "rhophiz", "rhophitheta", "rhophieta":
         for t2 in "xyz", "xytheta", "xyeta", "rhophiz", "rhophitheta", "rhophieta":
-            transformed1, transformed2 = (
-                getattr(v1, "to_" + t1)(),
-                getattr(v2, "to_" + t2)(),
+            taxis, tvec = (
+                getattr(axis, "to_" + t1)(),
+                getattr(vec, "to_" + t2)(),
             )
-            out = transformed1.cross(transformed2)
+            out = tvec.rotate_axis(taxis, 0.25)
             assert isinstance(out, vector.backends.object.VectorObject3D)
             assert isinstance(out.azimuthal, vector.backends.object.AzimuthalObjectXY)
             assert isinstance(
                 out.longitudinal, vector.backends.object.LongitudinalObjectZ
             )
-            assert (out.x, out.y, out.z) == pytest.approx((-0.03, 0.06, -0.03))
+            assert out.x == pytest.approx(0.37483425404335763)
+            assert out.y == pytest.approx(0.5383405688588193)
+            assert out.z == pytest.approx(0.5828282027463345)
 
 
 def test_spatial_numpy():
-    v1 = vector.backends.numpy.VectorNumpy3D(
+    axis = vector.backends.numpy.VectorNumpy3D(
         [(0.1, 0.2, 0.3)],
         dtype=[("x", numpy.float64), ("y", numpy.float64), ("z", numpy.float64)],
     )
-    v2 = vector.backends.numpy.VectorNumpy3D(
+    vec = vector.backends.numpy.VectorNumpy3D(
         [(0.4, 0.5, 0.6)],
         dtype=[("x", numpy.float64), ("y", numpy.float64), ("z", numpy.float64)],
     )
-    out = v1.cross(v2)
+    out = vec.rotate_axis(axis, 0.25)
     assert isinstance(out, vector.backends.numpy.VectorNumpy3D)
     assert out.dtype.names == ("x", "y", "z")
-    assert (out[0].x, out[0].y, out[0].z) == pytest.approx((-0.03, 0.06, -0.03))
+    assert out[0].x == pytest.approx(0.37483425404335763)
+    assert out[0].y == pytest.approx(0.5383405688588193)
+    assert out[0].z == pytest.approx(0.5828282027463345)
 
     for t1 in "xyz", "xytheta", "xyeta", "rhophiz", "rhophitheta", "rhophieta":
         for t2 in "xyz", "xytheta", "xyeta", "rhophiz", "rhophitheta", "rhophieta":
-            transformed1, transformed2 = (
-                getattr(v1, "to_" + t1)(),
-                getattr(v2, "to_" + t2)(),
+            taxis, tvec = (
+                getattr(axis, "to_" + t1)(),
+                getattr(vec, "to_" + t2)(),
             )
-            out = transformed1.cross(transformed2)
+            out = tvec.rotate_axis(taxis, 0.25)
             assert isinstance(out, vector.backends.numpy.VectorNumpy3D)
             assert out.dtype.names == ("x", "y", "z")
-            assert (out[0].x, out[0].y, out[0].z) == pytest.approx((-0.03, 0.06, -0.03))
+            assert out[0].x == pytest.approx(0.37483425404335763)
+            assert out[0].y == pytest.approx(0.5383405688588193)
+            assert out[0].z == pytest.approx(0.5828282027463345)
 
 
 def test_lorentz_object():
-    v1 = vector.backends.object.VectorObject4D(
+    axis = vector.backends.object.VectorObject4D(
         azimuthal=vector.backends.object.AzimuthalObjectXY(0.1, 0.2),
         longitudinal=vector.backends.object.LongitudinalObjectZ(0.3),
         temporal=vector.backends.object.TemporalObjectT(99),
     )
-    v2 = vector.backends.object.VectorObject4D(
+    vec = vector.backends.object.VectorObject4D(
         azimuthal=vector.backends.object.AzimuthalObjectXY(0.4, 0.5),
         longitudinal=vector.backends.object.LongitudinalObjectZ(0.6),
         temporal=vector.backends.object.TemporalObjectT(99),
     )
     with pytest.raises(TypeError):
-        out = v1.cross(v2)
-    v1, v2 = v1.to_Vector3D(), v2.to_Vector3D()
-    out = v1.cross(v2)
-    assert isinstance(out, vector.backends.object.VectorObject3D)
+        out = vec.rotate_axis(axis, 0.25)
+    out = vec.rotate_axis(axis.to_Vector3D(), 0.25)
+    assert isinstance(out, vector.backends.object.VectorObject4D)
     assert isinstance(out.azimuthal, vector.backends.object.AzimuthalObjectXY)
     assert isinstance(out.longitudinal, vector.backends.object.LongitudinalObjectZ)
-    assert (out.x, out.y, out.z) == pytest.approx((-0.03, 0.06, -0.03))
+    assert hasattr(out, "temporal")
+    assert out.x == pytest.approx(0.37483425404335763)
+    assert out.y == pytest.approx(0.5383405688588193)
+    assert out.z == pytest.approx(0.5828282027463345)
 
     for t1 in (
         "xyz",
         "xytheta",
         "xyeta",
         "rhophiz",
         "rhophitheta",
         "rhophieta",
     ):
         for t2 in (
-            "xyz",
-            "xytheta",
-            "xyeta",
-            "rhophiz",
-            "rhophitheta",
-            "rhophieta",
+            "xyzt",
+            "xythetat",
+            "xyetat",
+            "rhophizt",
+            "rhophithetat",
+            "rhophietat",
+            "xyztau",
+            "xythetatau",
+            "xyetatau",
+            "rhophiztau",
+            "rhophithetatau",
+            "rhophietatau",
         ):
-            transformed1, transformed2 = (
-                getattr(v1, "to_" + t1)(),
-                getattr(v2, "to_" + t2)(),
+            taxis, tvec = (
+                getattr(axis, "to_" + t1)(),
+                getattr(vec, "to_" + t2)(),
             )
-            out = transformed1.cross(transformed2)
-            assert isinstance(out, vector.backends.object.VectorObject3D)
+            out = tvec.rotate_axis(taxis, 0.25)
+            assert isinstance(out, vector.backends.object.VectorObject4D)
             assert isinstance(out.azimuthal, vector.backends.object.AzimuthalObjectXY)
             assert isinstance(
                 out.longitudinal, vector.backends.object.LongitudinalObjectZ
             )
-            assert (out.x, out.y, out.z) == pytest.approx((-0.03, 0.06, -0.03))
+            assert hasattr(out, "temporal")
+            assert out.x == pytest.approx(0.37483425404335763)
+            assert out.y == pytest.approx(0.5383405688588193)
+            assert out.z == pytest.approx(0.5828282027463345)
 
 
 def test_lorentz_numpy():
-    v1 = vector.backends.numpy.VectorNumpy3D(
+    axis = vector.backends.numpy.VectorNumpy4D(
         [(0.1, 0.2, 0.3, 99)],
         dtype=[
             ("x", numpy.float64),
             ("y", numpy.float64),
             ("z", numpy.float64),
             ("t", numpy.float64),
         ],
     )
-    v2 = vector.backends.numpy.VectorNumpy4D(
+    vec = vector.backends.numpy.VectorNumpy4D(
         [(0.4, 0.5, 0.6, 99)],
         dtype=[
             ("x", numpy.float64),
             ("y", numpy.float64),
             ("z", numpy.float64),
             ("t", numpy.float64),
         ],
     )
     with pytest.raises(TypeError):
-        out = v1.cross(v2)
-    v1, v2 = v1.to_Vector3D(), v2.to_Vector3D()
-    out = v1.cross(v2)
-    assert isinstance(out, vector.backends.numpy.VectorNumpy3D)
-    assert out.dtype.names == ("x", "y", "z")
-    assert out.tolist() == pytest.approx([(-0.03, 0.06, -0.030000000000000013)])
+        out = vec.rotate_axis(axis, 0.25)
+    out = vec.rotate_axis(axis.to_Vector3D(), 0.25)
+    assert isinstance(out, vector.backends.numpy.VectorNumpy4D)
+    assert out.dtype.names == ("x", "y", "z", "t")
+    assert out[0].x == pytest.approx(0.37483425404335763)
+    assert out[0].y == pytest.approx(0.5383405688588193)
+    assert out[0].z == pytest.approx(0.5828282027463345)
 
     for t1 in (
         "xyz",
         "xytheta",
         "xyeta",
         "rhophiz",
         "rhophitheta",
         "rhophieta",
     ):
         for t2 in (
-            "xyz",
-            "xytheta",
-            "xyeta",
-            "rhophiz",
-            "rhophitheta",
-            "rhophieta",
+            "xyzt",
+            "xythetat",
+            "xyetat",
+            "rhophizt",
+            "rhophithetat",
+            "rhophietat",
+            "xyztau",
+            "xythetatau",
+            "xyetatau",
+            "rhophiztau",
+            "rhophithetatau",
+            "rhophietatau",
         ):
-            transformed1, transformed2 = (
-                getattr(v1, "to_" + t1)(),
-                getattr(v2, "to_" + t2)(),
-            )
-            out = transformed1.cross(transformed2)
-            assert isinstance(out, vector.backends.numpy.VectorNumpy3D)
-            assert out.dtype.names == ("x", "y", "z")
-            assert (out[0].x, out[0].y, out[0].z) == pytest.approx((-0.03, 0.06, -0.03))
+            taxis, tvec = (
+                getattr(axis, "to_" + t1)(),
+                getattr(vec, "to_" + t2)(),
+            )
+            out = tvec.rotate_axis(taxis, 0.25)
+            assert isinstance(out, vector.backends.numpy.VectorNumpy4D)
+            assert out.dtype.names in {
+                ("x", "y", "z", "t"),
+                ("x", "y", "z", "tau"),
+            }
+            assert out[0].x == pytest.approx(0.37483425404335763)
+            assert out[0].y == pytest.approx(0.5383405688588193)
+            assert out[0].z == pytest.approx(0.5828282027463345)
```

### Comparing `vector-1.3.1/tests/compute/spatial/test_deltaR.py` & `vector-1.4.0/tests/compute/spatial/test_deltaR.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_deltaR2.py` & `vector-1.4.0/tests/compute/spatial/test_deltaR2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_deltaangle.py` & `vector-1.4.0/tests/compute/spatial/test_deltaangle.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_deltaeta.py` & `vector-1.4.0/tests/compute/spatial/test_deltaeta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_eta.py` & `vector-1.4.0/tests/compute/spatial/test_eta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_mag.py` & `vector-1.4.0/tests/compute/spatial/test_mag.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_mag2.py` & `vector-1.4.0/tests/compute/spatial/test_mag2.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_rotateX.py` & `vector-1.4.0/tests/compute/spatial/test_rotateX.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_rotateY.py` & `vector-1.4.0/tests/compute/spatial/test_rotateY.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_rotate_euler.py` & `vector-1.4.0/tests/compute/spatial/test_rotate_euler.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_rotate_quaternion.py` & `vector-1.4.0/tests/compute/spatial/test_rotate_quaternion.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_theta.py` & `vector-1.4.0/tests/compute/spatial/test_theta.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/compute/spatial/test_z.py` & `vector-1.4.0/tests/compute/spatial/test_z.py`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/samples/issue-161-v2.pkl` & `vector-1.4.0/tests/samples/issue-161-v2.pkl`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/tests/samples/issue-161.pkl` & `vector-1.4.0/tests/samples/issue-161.pkl`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/.gitignore` & `vector-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/LICENSE` & `vector-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector-1.3.1/README.md` & `vector-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 Main features of Vector:
 
 - Pure Python with NumPy as its only dependency. This makes it easier to install.
 - Vectors may be represented in a variety of coordinate systems: Cartesian, cylindrical, pseudorapidity, and any combination of these with time or proper time for Lorentz vectors. In all, there are 12 coordinate systems: {_x_-_y_ vs _ρ_-_φ_ in the azimuthal plane} × {_z_ vs _θ_ vs _η_ longitudinally} × {_t_ vs _τ_ temporally}.
 - Uses names and conventions set by [ROOT](https://root.cern/)'s [TLorentzVector](https://root.cern.ch/doc/master/classTLorentzVector.html) and [Math::LorentzVector](https://root.cern.ch/doc/master/classROOT_1_1Math_1_1LorentzVector.html), as well as [scikit-hep/math](https://github.com/scikit-hep/scikit-hep/tree/master/skhep/math), [uproot-methods TLorentzVector](https://github.com/scikit-hep/uproot3-methods/blob/master/uproot3_methods/classes/TLorentzVector.py), [henryiii/hepvector](https://github.com/henryiii/hepvector), and [coffea.nanoevents.methods.vector](https://coffeateam.github.io/coffea/modules/coffea.nanoevents.methods.vector.html).
 - Implemented on a variety of backends:
   - pure Python objects
+  - [SymPy](https://www.sympy.org/en/index.html) vectors
   - NumPy arrays of vectors (as a [structured array](https://numpy.org/doc/stable/user/basics.rec.html) subclass)
   - [Awkward Arrays](https://awkward-array.org/) of vectors
   - potential for more: CuPy, TensorFlow, Torch, JAX...
-- NumPy/Awkward backends also implemented in [Numba](https://numba.pydata.org/) for JIT-compiled calculations on vectors.
+- Awkward backend also implemented in [Numba](https://numba.pydata.org/) for JIT-compiled calculations on vectors.
+- [JAX](https://awkward-array.org/doc/main/user-guide/how-to-specialize-differentiate-jax.html) and [Dask](https://dask-awkward.readthedocs.io/en/stable/) support through Awkward Arrays.
 - Distinction between geometrical vectors, which have a minimum of attribute and method names, and vectors representing momentum, which have synonyms like `pt` = `rho`, `energy` = `t`, `mass` = `tau`.
 
 ## Installation
 
 To install, use `pip install vector` or your favorite way to install in an environment.
 
 ## Overview
@@ -54,15 +56,15 @@
 - `vector.obj` to make a pure Python vector object,
 - `vector.arr` to make a NumPy array of vectors (or `array`, lowercase, like `np.array`),
 - `vector.awk` to make an Awkward Array of vectors (or `Array`, uppercase, like `ak.Array`).
 - `vector.zip` to make an Awkward Array of vectors (similar to `ak.zip`)
 
 ### Pure Python vectors
 
-You can directly use the `VectorObject` classes to construct object type vectors:
+You can directly use the `VectorObject` and `MomentumObject` classes to construct object type vectors:
 
 ```python
 vector.VectorObject2D(x=1.1, y=2.2)
 vector.MomentumObject3D(px=1.1, py=2.2, pz=3.3)
 vector.VectorObject4D(x=1.1, y=2.2, eta=3.3, tau=4.4)
 ```
 
@@ -155,14 +157,88 @@
 vector.VectorObject2D.from_xy(1.1, 2.2)
 vector.MomentumObject3D.from_rhophiz(1.1, 2.2, 3.3)
 vector.VectorObject4D.from_xyetatau(1.1, 2.2, 3.3, 4.4)
 ```
 
 and so on, for all combinations of azimuthal, longitudinal, and temporal coordinates, geometric and momentum-flavored.
 
+### SymPy vectors
+
+> **Note:** Operations on SymPy vectors are only 100% compatible with numeric vectors (Python, NumPy, and Awkward backends) if the vectors are positive time-like, that is, if `t**2 > x**2 + y**2 + z**2`. The space-like and negative time-like cases have different sign conventions.
+
+You can directly use the `VectorSympy` and `MomentumSympy` classes to construct object type vectors:
+
+```python
+import sympy
+
+x, y, z, t, px, py, pz, eta, tau = sympy.symbols(
+    "x y z t px py pz eta tau",
+    real=True,  # see sympy assumptions to add more restrictions on the symbols
+)
+vector.VectorSympy2D(x=x, y=y)
+vector.MomentumSympy3D(px=px, py=py, pz=pz)
+vector.VectorSympy4D(x=x, y=y, eta=eta, tau=tau)
+```
+
+and so on for every class.
+
+```python
+# Test instance type for any level of granularity.
+(
+    # is a vector or array of vectors
+    isinstance(vector.VectorSympy2D(x=x, y=y), vector.Vector),
+    # is 2D (not 3D or 4D)
+    isinstance(vector.VectorSympy2D(x=x, y=y), vector.Vector2D),
+    # is a sympy vector (not an array)
+    isinstance(vector.VectorSympy2D(x=x, y=y), vector.VectorSympy),
+    # has momentum synonyms
+    isinstance(vector.MomentumSympy2D(px=px, py=py), vector.Momentum),
+    # has transverse plane (2D, 3D, or 4D)
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t), vector.Planar),
+    # has all spatial coordinates (3D or 4D)
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t), vector.Spatial),
+    # has temporal coordinates (4D)
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t), vector.Lorentz),
+    # azimuthal coordinate type
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t).azimuthal, vector.AzimuthalXY),
+    # longitudinal coordinate type
+    isinstance(
+        vector.VectorSympy4D(x=x, y=y, z=z, t=t).longitudinal, vector.LongitudinalZ
+    ),
+    # temporal coordinate type
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t).temporal, vector.TemporalT),
+)
+```
+
+Since `VectorSympy2D`, `VectorSympy3D`, `VectorSympy4D`, and their momentum equivalents operate on SymPy expressions, all of the normal SymPy methods and functions work on the results, coordinates, and the vectors.
+
+```python
+sympy.init_session()  # latex printing
+
+v1 = vector.VectorSympy2D(x=x, y=y)
+sympy.Eq(v1.rho, sympy.sqrt(x**2 + y**2))
+
+v2 = vector.VectorSympy4D(x=x, y=y, z=z, t=t)
+v2.to_rhophithetatau().tau
+
+values = {x: 3, y: 2, z: 1, t: 10}  # t**2 > x**2 + y**2 + z**2
+v2.is_timelike()
+v2.is_timelike().subs(values)
+
+v2.to_rhophithetatau().tau.subs(values).evalf()
+
+v2.boost(v2.to_beta3())
+v2.boost(v2.to_beta3()).t
+v2.boost(v2.to_beta3()).t.simplify()
+v2.boost(v2.to_beta3()).t.subs(values)
+v2.boost(v2.to_beta3()).t.subs(values).evalf()
+```
+
+All of the keyword arguments and rules that apply to `vector.obj` construction apply to `vector.VectorSympyND` and `vector.MomentumObjectND` objects.
+
 ### NumPy arrays of vectors
 
 You can directly use the `VectorNumpy` classes to construct object type vectors:
 
 ```python
 # NumPy-like arguments (literally passed through to NumPy)
 vector.VectorNumpy2D(
```

### Comparing `vector-1.3.1/pyproject.toml` & `vector-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,28 +50,32 @@
   "dask_awkward",
   "nox",
   'numba>=0.57; python_version < "3.12"',
   "papermill>=2.4",
   "pytest>=6",
   "pytest-cov>=3",
   "pytest-doctestplus",
+  "sympy",
 ]
 docs = [
   "awkward>=1.2",
   "ipykernel",
   "myst-parser>0.13",
   "nbsphinx",
   "Sphinx>=4",
   "sphinx-math-dollar",
   "sphinx_book_theme>=0.0.42",
   "sphinx_copybutton",
 ]
 numba = [
   'numba>=0.57; python_version < "3.12"',
 ]
+sympy = [
+  "sympy",
+]
 test = [
   "dask_awkward",
   "nox",
   "papermill>=2.4",
   "pytest>=6",
   "pytest-cov>=3",
   "pytest-doctestplus",
@@ -196,14 +200,15 @@
     "tests",
 ]
 markers = [
     "slow",
     "numba",
     "awkward",
     "dis",
+    "sympy",
 ]
 log_cli_level = "DEBUG"
 filterwarnings = [
     "error",
     "ignore::DeprecationWarning",
     "ignore::UserWarning",
 ]
```

### Comparing `vector-1.3.1/PKG-INFO` & `vector-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: vector
-Version: 1.3.1
+Version: 1.4.0
 Summary: Vector classes and utilities
 Project-URL: Bug Tracker, https://github.com/scikit-hep/vector/issues
 Project-URL: Changelog, https://vector.readthedocs.io/en/latest/changelog.html
 Project-URL: Discussions, https://github.com/scikit-hep/vector/discussions
 Project-URL: Documentation, https://vector.readthedocs.io/
 Project-URL: Homepage, https://github.com/scikit-hep/vector
 Author-email: "Jim Pivarski, Henry Schreiner, Eduardo Rodrigues" <eduardo.rodrigues@cern.ch>
@@ -38,25 +38,28 @@
 Requires-Dist: dask-awkward; extra == 'dev'
 Requires-Dist: nox; extra == 'dev'
 Requires-Dist: numba>=0.57; (python_version < '3.12') and extra == 'dev'
 Requires-Dist: papermill>=2.4; extra == 'dev'
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest-doctestplus; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
+Requires-Dist: sympy; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: awkward>=1.2; extra == 'docs'
 Requires-Dist: ipykernel; extra == 'docs'
 Requires-Dist: myst-parser>0.13; extra == 'docs'
 Requires-Dist: nbsphinx; extra == 'docs'
 Requires-Dist: sphinx-book-theme>=0.0.42; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-math-dollar; extra == 'docs'
 Requires-Dist: sphinx>=4; extra == 'docs'
 Provides-Extra: numba
 Requires-Dist: numba>=0.57; (python_version < '3.12') and extra == 'numba'
+Provides-Extra: sympy
+Requires-Dist: sympy; extra == 'sympy'
 Provides-Extra: test
 Requires-Dist: dask-awkward; extra == 'test'
 Requires-Dist: nox; extra == 'test'
 Requires-Dist: papermill>=2.4; extra == 'test'
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest-doctestplus; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
@@ -89,18 +92,20 @@
 Main features of Vector:
 
 - Pure Python with NumPy as its only dependency. This makes it easier to install.
 - Vectors may be represented in a variety of coordinate systems: Cartesian, cylindrical, pseudorapidity, and any combination of these with time or proper time for Lorentz vectors. In all, there are 12 coordinate systems: {_x_-_y_ vs _ρ_-_φ_ in the azimuthal plane} × {_z_ vs _θ_ vs _η_ longitudinally} × {_t_ vs _τ_ temporally}.
 - Uses names and conventions set by [ROOT](https://root.cern/)'s [TLorentzVector](https://root.cern.ch/doc/master/classTLorentzVector.html) and [Math::LorentzVector](https://root.cern.ch/doc/master/classROOT_1_1Math_1_1LorentzVector.html), as well as [scikit-hep/math](https://github.com/scikit-hep/scikit-hep/tree/master/skhep/math), [uproot-methods TLorentzVector](https://github.com/scikit-hep/uproot3-methods/blob/master/uproot3_methods/classes/TLorentzVector.py), [henryiii/hepvector](https://github.com/henryiii/hepvector), and [coffea.nanoevents.methods.vector](https://coffeateam.github.io/coffea/modules/coffea.nanoevents.methods.vector.html).
 - Implemented on a variety of backends:
   - pure Python objects
+  - [SymPy](https://www.sympy.org/en/index.html) vectors
   - NumPy arrays of vectors (as a [structured array](https://numpy.org/doc/stable/user/basics.rec.html) subclass)
   - [Awkward Arrays](https://awkward-array.org/) of vectors
   - potential for more: CuPy, TensorFlow, Torch, JAX...
-- NumPy/Awkward backends also implemented in [Numba](https://numba.pydata.org/) for JIT-compiled calculations on vectors.
+- Awkward backend also implemented in [Numba](https://numba.pydata.org/) for JIT-compiled calculations on vectors.
+- [JAX](https://awkward-array.org/doc/main/user-guide/how-to-specialize-differentiate-jax.html) and [Dask](https://dask-awkward.readthedocs.io/en/stable/) support through Awkward Arrays.
 - Distinction between geometrical vectors, which have a minimum of attribute and method names, and vectors representing momentum, which have synonyms like `pt` = `rho`, `energy` = `t`, `mass` = `tau`.
 
 ## Installation
 
 To install, use `pip install vector` or your favorite way to install in an environment.
 
 ## Overview
@@ -121,15 +126,15 @@
 - `vector.obj` to make a pure Python vector object,
 - `vector.arr` to make a NumPy array of vectors (or `array`, lowercase, like `np.array`),
 - `vector.awk` to make an Awkward Array of vectors (or `Array`, uppercase, like `ak.Array`).
 - `vector.zip` to make an Awkward Array of vectors (similar to `ak.zip`)
 
 ### Pure Python vectors
 
-You can directly use the `VectorObject` classes to construct object type vectors:
+You can directly use the `VectorObject` and `MomentumObject` classes to construct object type vectors:
 
 ```python
 vector.VectorObject2D(x=1.1, y=2.2)
 vector.MomentumObject3D(px=1.1, py=2.2, pz=3.3)
 vector.VectorObject4D(x=1.1, y=2.2, eta=3.3, tau=4.4)
 ```
 
@@ -222,14 +227,88 @@
 vector.VectorObject2D.from_xy(1.1, 2.2)
 vector.MomentumObject3D.from_rhophiz(1.1, 2.2, 3.3)
 vector.VectorObject4D.from_xyetatau(1.1, 2.2, 3.3, 4.4)
 ```
 
 and so on, for all combinations of azimuthal, longitudinal, and temporal coordinates, geometric and momentum-flavored.
 
+### SymPy vectors
+
+> **Note:** Operations on SymPy vectors are only 100% compatible with numeric vectors (Python, NumPy, and Awkward backends) if the vectors are positive time-like, that is, if `t**2 > x**2 + y**2 + z**2`. The space-like and negative time-like cases have different sign conventions.
+
+You can directly use the `VectorSympy` and `MomentumSympy` classes to construct object type vectors:
+
+```python
+import sympy
+
+x, y, z, t, px, py, pz, eta, tau = sympy.symbols(
+    "x y z t px py pz eta tau",
+    real=True,  # see sympy assumptions to add more restrictions on the symbols
+)
+vector.VectorSympy2D(x=x, y=y)
+vector.MomentumSympy3D(px=px, py=py, pz=pz)
+vector.VectorSympy4D(x=x, y=y, eta=eta, tau=tau)
+```
+
+and so on for every class.
+
+```python
+# Test instance type for any level of granularity.
+(
+    # is a vector or array of vectors
+    isinstance(vector.VectorSympy2D(x=x, y=y), vector.Vector),
+    # is 2D (not 3D or 4D)
+    isinstance(vector.VectorSympy2D(x=x, y=y), vector.Vector2D),
+    # is a sympy vector (not an array)
+    isinstance(vector.VectorSympy2D(x=x, y=y), vector.VectorSympy),
+    # has momentum synonyms
+    isinstance(vector.MomentumSympy2D(px=px, py=py), vector.Momentum),
+    # has transverse plane (2D, 3D, or 4D)
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t), vector.Planar),
+    # has all spatial coordinates (3D or 4D)
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t), vector.Spatial),
+    # has temporal coordinates (4D)
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t), vector.Lorentz),
+    # azimuthal coordinate type
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t).azimuthal, vector.AzimuthalXY),
+    # longitudinal coordinate type
+    isinstance(
+        vector.VectorSympy4D(x=x, y=y, z=z, t=t).longitudinal, vector.LongitudinalZ
+    ),
+    # temporal coordinate type
+    isinstance(vector.VectorSympy4D(x=x, y=y, z=z, t=t).temporal, vector.TemporalT),
+)
+```
+
+Since `VectorSympy2D`, `VectorSympy3D`, `VectorSympy4D`, and their momentum equivalents operate on SymPy expressions, all of the normal SymPy methods and functions work on the results, coordinates, and the vectors.
+
+```python
+sympy.init_session()  # latex printing
+
+v1 = vector.VectorSympy2D(x=x, y=y)
+sympy.Eq(v1.rho, sympy.sqrt(x**2 + y**2))
+
+v2 = vector.VectorSympy4D(x=x, y=y, z=z, t=t)
+v2.to_rhophithetatau().tau
+
+values = {x: 3, y: 2, z: 1, t: 10}  # t**2 > x**2 + y**2 + z**2
+v2.is_timelike()
+v2.is_timelike().subs(values)
+
+v2.to_rhophithetatau().tau.subs(values).evalf()
+
+v2.boost(v2.to_beta3())
+v2.boost(v2.to_beta3()).t
+v2.boost(v2.to_beta3()).t.simplify()
+v2.boost(v2.to_beta3()).t.subs(values)
+v2.boost(v2.to_beta3()).t.subs(values).evalf()
+```
+
+All of the keyword arguments and rules that apply to `vector.obj` construction apply to `vector.VectorSympyND` and `vector.MomentumObjectND` objects.
+
 ### NumPy arrays of vectors
 
 You can directly use the `VectorNumpy` classes to construct object type vectors:
 
 ```python
 # NumPy-like arguments (literally passed through to NumPy)
 vector.VectorNumpy2D(
```

