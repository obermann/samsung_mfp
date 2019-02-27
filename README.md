# samsung_mfp
SANE backend for Samsung SCX-4600 MFP

[Scanner Access Now Easy (SANE)](http://www.sane-project.org/) recomended backend for Samsung SCX-4600
is xerox_mfp and it was not good for me. So I took xerox_mfp.c form
[SANE version 1.0.21](https://gitlab.com/sane-project/backends/tags/RELEASE_1_0_21),
renamed it to samsung_mfp and made it perfect for Samsung SCX-4600:

* Added Color
* Added 1200dpi
* Removed right-side white band
* Removed top-side white band in mono images

All changes are visible in a diff with the initial commit.

Note. samsung_mfp.conf.in and xerox_mfp.conf.in overlap in defining scanners USB identification,
so you may need to solve the conflict, e.g. disabling one or another backend.
