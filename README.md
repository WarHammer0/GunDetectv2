# GunDetectv2
Gun detection inference graph Version 2. 150,000 images manually tagged, trained on a Power9 AC922 with 2x Nvidia Tesla V100

Tensorflow weapon detection module, v1. Trained 2,000,000 steps on Power9 hardware with 2x Nvidia Tesla v100s. Haven't benchmarked it yet, but it appears to be fairly accurate.

This was trained on a hand-tagged dataset of 2,000 images, augmented to 150,000 with random crop, rotate, and color modification with 7 types of weapons: AR-Type rifle, Ak-type rifle, shotgun, hunting rifle, mp5, pistol, holstered pistol

The recognition between pistol and holstered pistol is spotty, so if the functionality is not required, I'd recommend simply editing your labelmap to detect them both as the same. MP5 for now will only detect MP5-style submachineguns, but will likely expand to include all submachine guns in a future update

Hope someone can get some use out of this!
