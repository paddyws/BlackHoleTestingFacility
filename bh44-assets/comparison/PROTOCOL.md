# Raw dominant versus all-six mass comparison
Declared2026-10-17T21:15Z before calculating this two-method result. This follows explicit user request and retains all previously frozen definitions. The coordinator has seen earlier three-case baseline validation; this is an exploratory comparison, not a new blind confirmatory test.

Primary cohort: identical galaxies with finite raw unscreened dominant-mode absolute pitch and finite baseline-valid all-six predictor, valid baseline disk geometry/input eligibility, and direct reference mass. Expected33; preserve all44 coverage rows. The all-six predictor is abs(sum A_m*SIGNED_pitch_m / sum A_m), not mean absolute pitch. Never suppress cancellation or choose a sign based on mass.

Fit unweighted log10 black-hole mass versus absolute angle, with an intercept and slope. Report pitch–mass Pearson/Spearman, in-sample slope/scatter, leave-one-galaxy-out MAE/RMSE/residualSD, prediction–mass correlations, and intercept-only leave-one-out mean baseline. Report mass errors unchanged but do not use them as regression weights or claim measurement-error correction.

Paired5000 galaxy bootstrap of frozen out-of-fold residual vectors, seed20261017; report percentile95% intervals for differences, explicitly conditional on predictions, not calibrated generalization intervals. Delete-one-galaxy jackknife reruns all LOOCV fits. Minimum8 for these descriptive intervals. No multiplicity correction, no model tuning, no selection by target value or residual.

Predeclared secondary flag sensitivities, all reported: fitted inclination<50degrees; excluding documented residual-artifact cases NGC1097 (large-scale background residuals), NGC3031 (remaining SDSS diagonal sky seams), NGC4736 (negative sky patches), NGC5055 (horizontal sky seam), NGC6264 (detector line); and both restrictions. This artifact list comes from existing geometry review notes, not target information. It is a conservative stress test, not a claim that every other image is artifact-free. High inclination was not excluded from the primary comparison. Show sample counts and every omitted name.

No original frozen measurements or image-only choices are altered. New raw comparison outputs are separate from the historical screened-maximum baseline.
