# BlackHoleTestingFacility

Public inspection of the exact 44-object Davis et al. (2017) spiral-galaxy / black-hole-mass sample.

- index.html: frozen image-derived pitch measurements, literature reference |pitch| and 1-sigma errors for all 44 objects, inclinations, flags, and exploratory identical-cohort mass comparison.
- inspection.html: all 232 available rendered image displays across 43 external galaxies, including failure cases; the Milky Way has no external whole-disk view.
- fits.html: 43 external survey FITS cutout links and adopted-analysis input hashes. Exact archived processed inputs and masks are not included.

## Scientific provenance

Published pitch values are unsigned magnitudes, not new FFT results. They come from Davis, Graham & Seigar (2017), MNRAS 471,2187–2203, Table 1: https://doi.org/10.1093/mnras/stx1794 ; author manuscript v3 https://arxiv.org/pdf/1707.04001v3 . Original measurement references, methods, tracers, telescope/filter and uncertainties are recorded per galaxy in bh44-assets/literature_pitch_reference.json and.csv. The Milky Way value is a literature meta-analysis; Cygnus A refers to nuclear arms, not the whole host disk.

Survey displays and monochromatic inputs originate from the DESI Legacy Imaging Surveys viewer (including the selected SDSS layers) and CDS HiPS2FITS services (selected Pan-STARRS, DECaPS and SkyMapper layers). Per-galaxy actual survey/filter/acquisition URLs and image hashes are retained in bh44-assets/preview-data.json. See https://www.legacysurvey.org/acknowledgment/ and https://aladin.cds.unistra.fr/hips/ . Scientific arrays were frozen before the original mass comparison. The public addition only joins published pitch references and preserves the new raw and baseline measurements.

Raw strongest mode is the unfiltered largest Fourier amplitude across tested m=1–6 at the fixed annulus. Quality flags remain visible. The all-six estimate is the amplitude-weighted signed mean; opposite signs can cancel. Numerical maxima and overlays do not automatically trace physical spiral arms. Invalid geometry and support failures remain explicitly labeled.

The separate 33-galaxy exploratory mass comparison establishes no clear winning method; neither improves the mean-mass-only baseline in this sample. It does not establish that physical spiral pitch in general has no relationship with black-hole mass. Exact results, protocol, report and prediction tables are included under bh44-assets/comparison.

## Display and access

Static files and relative paths are compatible with GitHub Pages project hosting. Images are the previously verified full-resolution lossless web displays or byte-identical JPEG context images. No private service links, authentication material, internal account IDs, or unrelated 96-galaxy catalogue are included. Optional geometry-QA composites and raw FITS/masks are not embedded.

## Published black-hole masses

All 44 galaxies include the adopted directly measured black-hole mass from Table 1 of Davis et al. (2017), asymmetric 1-sigma errors in dex, the decoded measurement technique and original source citations. These are distance-adjusted adopted literature masses, not pitch-predicted masses. Central solar-mass values and converted upper/lower uncertainties are also in bh44-assets/black_hole_mass_reference.json and .csv. The source table’s apparent NGC 4388 reference mismatch is preserved and explicitly flagged, rather than silently corrected; NGC 4736 and NGC 4826 include the table’s private-communication provenance.
