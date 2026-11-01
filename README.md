# Computer Graphics Labs (Wolfram Mathematica)

Lab work from the Computer Graphics course at SIIT (Year 2, Term 2). Everything is written in the Wolfram Language. The labs build from parametric curves and spline interpolation up to 2D/3D geometric transformations, texture mapping, and interactive animations.

**Viewing:** every notebook has a PDF next to it that can be read directly on GitHub. To run the code, open the `.nb` files in [Mathematica](https://www.wolfram.com/mathematica/) or the free [Wolfram Player](https://www.wolfram.com/player/); the `Manipulate` panels and sliders are interactive there.

## Labs

| Lab | Topics | Files |
|---|---|---|
| [Lab 5: Splines and 3D Parametric Curves](labs/lab05-splines-and-3d-curves) | Surfaces of revolution, 3D helices, spline interpolation through 2D/3D points, tracing a horse outline with a parametric spline and placing it on a plane in 3D, interactive controls (`PopupMenu`, `Slider`, `Slider2D`, `VerticalSlider`) | `.nb` `.pdf` |
| [Lab 6: Modules, Interpolation and Texture Mapping](labs/lab06-modules-and-texture-mapping) | `Module` scoping and higher-order functions, functions that return interpolating functions, texture-mapping images onto a parametric torus that travels along a spline path, reconstructing a surface from sampled data with `ListInterpolation`, placing spheres on a surface grid | `.nb` `.pdf` |
| [Lab 7: Trajectories and Moving Objects](labs/lab07-trajectories-and-moving-objects) | List processing with `Module` (primes, sums, prime-counting curve fit), piecewise paths with `Which`, step-function paths, polygons that rotate while following a closed spline, surfaces moving along 3D trajectories, reusable animation functions | `.nb` `.pdf` |
| [Lab 8: 2D Geometric Transformations](labs/lab08-2d-geometric-transformations) | Composing `RotationTransform` and `TranslationTransform`, orbiting with and without self-rotation, rotation about an arbitrary center, objects following parabolic and figure-eight trajectories, a reusable `Module`-based animation function | `.nb` `.pdf` |
| [Lab 9: Animation and Collision](labs/lab09-animation-and-collision) | Moving an imported 3D model along a polynomial space curve, precomputed trajectories, start/stop animation loops, a ball bouncing inside a box and inside a circle with wall reflection | `.nb` `.pdf` |
| [Lab 10: 3D Rotations and Interactive Controls](labs/lab10-3d-rotations-and-controls) | Rotating surfaces and polyhedra about chosen axes, a torus with an orbiting sphere, a ring rotating through a Menger sponge, rotating a spiral about a pivot chosen with sliders, a highlighted segment travelling along a trefoil knot | `.nb` `.pdf` |

## Practice

| Notebook | Contents |
|---|---|
| Final Exam Review ([pdf](practice/final-review.pdf), [nb](practice/final-review.nb)) | Final-exam review that combines techniques from Labs 7 and 10 (surface following a helix, objects on 3D spline paths, prime plots, ladder path, rotating shape menu, torus/sphere system, trefoil knot) |
| Final Exam Practice ([pdf](practice/final-practice.pdf), [nb](practice/final-practice.nb)) | Practice problems: a rotating 3D object assembled from primitives, and a shape picker that orbits the chosen shape |
| Mathematica Basics ([pdf](practice/mathematica-basics.pdf), [nb](practice/mathematica-basics.nb)) | Introductory exercises: plotting, styling, matrices, 3D plots, parametric curves |

## Notes

- **Labs 9 and 10 load external 3D models** (`spikeymodel.stl` and `Menger_sponge.stl`) that are not included in this repository. To re-run those sections, put the files in the same folder as the notebook; the notebooks set the working directory to their own folder.
- The PDFs come from a fresh top-to-bottom evaluation of each notebook, so random colors may differ from the original run. For the Lab 9 and 10 PDFs, the two models were replaced with stand-ins generated from Wolfram's built-in `PolyhedronData["Spikey"]` and `MengerMesh`, so those shapes may look different from the original models. The Lab 9 and 10 notebooks keep their original saved outputs.

## Structure

```
labs/
  lab05-splines-and-3d-curves/
  lab06-modules-and-texture-mapping/
  lab07-trajectories-and-moving-objects/
  lab08-2d-geometric-transformations/
  lab09-animation-and-collision/
  lab10-3d-rotations-and-controls/
practice/
```
