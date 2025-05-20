# MyLittlePony-healpy-cmaps
These are custom made colour maps used to plot Healpix maps in Mollweide projection, that I made in honour of my childhood favourite MLP characters. 

# 🎨 Custom Colormaps for Healpy and Matplotlib

This repository contains custom colormaps designed for use with [Healpy](https://healpy.readthedocs.io/en/latest/) and general-purpose plotting.

The goal is to provide visually distinct color palettes for sky maps and other scientific plots — especially helpful for radio astronomy, cosmology, and CMB/foreground studies, but a little bit more unique and with a twist!

---

## 🗂️ Contents

- `colormaps/` — Python scripts or `.npy` files containing colormap definitions
- `examples/` — Example notebooks and scripts to demonstrate usage
- `LICENSE` — Creative Commons Attribution 4.0 License (CC BY 4.0)

---

## 🔧 How to Use

You can import these colormaps directly in Python:

```python
import matplotlib.pyplot as plt
import numpy as np
from my_colormaps import newcmp  # or however you structure your import

# Apply to a Healpy map
import healpy as hp
hp.mollview(my_map, cmap=newcmp)

# Or a regular matplotlib plot
plt.imshow(my_image, cmap=newcmp)
