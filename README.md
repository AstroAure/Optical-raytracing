# Optical raytracing in Python

This package in the making offers the possibility to **create optical setup** and **visualize the light rays going through it**.

It originated as a way to better understand how instruments in astronomy worked, and allow to design them for amateur scientific endeavours. However, this package can be used in very different fields !

## What makes this package special ?

1. It allows for modeling setup that use **dispersive elements** (gratings, *prism*, *grism*), and soon will also take dispersion in lenses into account.

2. The optical elements geometry are **described by parameterized curves** allowing for exact interaction bewteen light rays and optical elements. This gives way better results than using discretized elements. To make this easy to use, each optical element is defined by one set of equations, that are automatically modified to place it where and in the orientation you want. The most common optical elements are already implemented, but you can add whatever you want with th method !

## Optical elements

This package integrates the following optical elements. The elements in *italic* aren't developed yet but should be added soon.

* **Mirror**:
    * Flat
    * Parabolic
    * Hyperbolic
    * *Spherical*

* **Lens**[^1]:
    * Spherical
    * *Doublet*
    * *Triplet*

* **Dispersive**:
    * Reflection grating
    * Transmission grating
    * *Prism*
    * *Grism*

[^1]: The lenses don't take dispersion into account yet (the index of refraction is constant regardless of the wavelength).
