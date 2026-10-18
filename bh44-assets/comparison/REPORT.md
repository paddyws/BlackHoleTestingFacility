# Raw dominant pitch versus all-six pitch: black-hole mass

## Main result
On the identical 33-galaxy common cohort, both estimators have almost no observed linear or rank correlation with log black-hole mass. The all-six estimator has a slightly smaller prediction error, but the difference is tiny and uncertain. Neither improves the mean-mass-only baseline in this experiment.

| Measure | Raw dominant mode | Magnitude of all-six signed mean | Mean-mass-only baseline |
|---|---:|---:|---:|
| Galaxies | 33 | 33 | 33 |
| Pearson pitch–mass r | −0.037 | −0.082 | — |
| Spearman pitch–mass rho | −0.041 | −0.082 | — |
| Held-out RMSE (dex) | 0.743 | 0.735 | 0.719 |
| Held-out MAE (dex) | 0.609 | 0.608 | 0.589 |
| Held-out residual SD (dex) | 0.754 | 0.746 | 0.730 |

Each prediction is from an unweighted straight-line fit of log10(MBH/Msun) against absolute pitch trained on the other 32 galaxies. The baseline predicts the other galaxies' mean log mass. Error bars on the scatter plot show the supplied mass uncertainties; those errors are retained but are not regression weights, and uncertainties in either axis are not propagated.

Raw-minus-all-six RMSE difference is +0.0077 dex. The paired bootstrap descriptive 95% interval is −0.0121 to +0.0263 dex; the full-refit delete-one jackknife interval is −0.0177 to +0.0330 dex. Both span zero. The bootstrap resamples paired frozen held-out residual vectors; it is conditional on those predictions, not a calibrated generalization interval. No method is established as better.

## What “all six” means
It is the absolute value of the amplitude-weighted SIGNED mean across m=1–6. It is not the weighted mean of absolute mode pitches. Opposite winding signs can cancel and yield a small number without describing a tightly wound physical arm. The original shares, cancellation flags and p=0 rules are unchanged. Raw dominant means the unfiltered largest Fourier amplitude at the same default annulus. The displayed raw value does not need to pass the earlier peak-quality screen.

## Secondary quality-flag sensitivities
These subsets were declared before calculating this comparison and are all shown. None gives a statistically clear two-method ranking; every paired RMSE-difference interval spans zero.

| Subset | N | Dominant RMSE | All-six RMSE | Mean-only RMSE |
|---|---:|---:|---:|---:|
| Full common cohort | 33 | 0.743 | 0.735 | 0.719 |
| Fitted inclination <50° | 12 | 0.698 | 0.707 | 0.654 |
| Exclude documented residual-artifact cases | 28 | 0.644 | 0.656 | 0.644 |
| Both restrictions | 9 | 0.698 | 0.574 | 0.639 |

The last, smallest subset has a larger apparent all-six advantage, but its paired bootstrap interval remains broad (raw-minus-all-six RMSE: −0.049 to +0.285 dex) and the refit jackknife is broader still. It is not a basis for choosing that subset or claiming superiority.

The fixed artifact stress-test excludes NGC1097, NGC3031, NGC4736, NGC5055 and NGC6264 for previously documented residual background/seam/detector-line issues. This is not a claim that all other images are artifact-free. The primary result retains high-inclination cases and these flagged artifacts. All subset names, removed cases, coverage and numerical results are in comparison.json and cohort_and_flags.csv.

## Limits
This tests these specific image-derived estimators and heterogeneous survey images, not whether every possible spiral-pitch measurement predicts mass. The 33 common galaxies exclude invalid baseline geometry/input cases and undefined six-mode means. They are not an unbiased complete sample of spirals. Measurements and masks were frozen before original mass access; this later comparison follows a user-requested estimator change, and is exploratory internal validation, not an external confirmatory benchmark. No annulus, parameter or subset was selected using the new target correlation. No original frozen measurements were altered.

Pitch–mass correlations are the appropriate association summaries here. Correlation of leave-one-out predictions with targets is included for completeness in JSON but must not be interpreted as a physical anticorrelation: even leave-one-out mean predictions can be negatively coupled to their held-out target.

## Files
- raw_vs_all6_mass.png: two scatter plots and identical-cohort held-out RMSE
- metric_summary.csv: primary and all secondary metrics
- heldout_predictions.csv: every prediction, residual and training count
- cohort_and_flags.csv: all 44 objects, inclusion, flags and mass errors
- comparison.json: exact values, correlations, fits, paired bootstrap and jackknife outputs, provenance hashes
- PROTOCOL.md: declared comparison and sensitivity rules
