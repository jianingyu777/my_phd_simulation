# Evidence Package A final v1

## Goal

Evidence Package A validates whether kilometer-scale public satellite sensors retain SDGSAT-observed contrail BTD signals. This final package integrates the already audited MODIS, MODIS morphology, MODIS cloud-product, MODIS-GOES joint, GOES parallax QC, and formal GOES parallax-corrected results.

## Completed Sensors

- MODIS Terra: polar-orbiting thermal BTD and MOD06 cloud-product retrieval-floor analysis.
- GOES ABI: geostationary BTD analysis with formal H10 parallax-corrected object support and H8/H10/H12 height sensitivity.

## Data Volume

- MODIS v1: 81 processed scenes, 3830 objects.
- MODIS-GOES joint v2.1: 61.0 GOES H10 scenes, 5202.0 objects, 2847.0 both-usable H10 objects.
- Common processed MODIS-GOES scenes: 53.

## Four Metrics

- Detection retention: MODIS 0.015097; GOES H10 0.038002.
- BTD signal-floor fraction: MODIS 0.984903; GOES H10 0.961998; both floor H10 0.938532.
- Signal retention median ref005: MODIS 0.445971; GOES H10 1.649003.
- MOD06 product retrieval-floor fraction among evaluable objects: 0.629630.
- Morphology-specific loss: rule-based morphology groups show high signal-floor fractions for both MODIS and GOES H10.

## GOES Parallax Correction

GOES v2.1 uses formal line-of-sight parallax projection. H10 is the primary result; H8/H10/H12 sensitivity is reported because GOES signal-retention magnitude depends on assumed cloud-top height. The H8/H10/H12 GOES ref005 retention medians are 1.533443, 1.649003, and 1.649801.

## Key Conclusions

MODIS and GOES both show very low BTD-threshold detection retention and very high BTD signal-floor fractions for SDGSAT contrail objects. MODIS cloud-product analysis shows retrieval-floor behavior in MOD06 among evaluable objects. High loss is observed across rule-based morphology groups.

## Limitations

- GOES cloud-product retrieval-floor analysis is not yet included.
- GOES signal-retention magnitude should be reported as a height-sensitivity range.
- Morphology labels are rule-based groups, not manual truth labels.
- The common processed scene count is 53, which reaches the minimum and 50-scene standard but not the 100+ common-scene target.

## Recommended Next Steps

- GOES-only full 131 scene run.
- SEVIRI IODC branch.
- Expansion toward 100+ common scenes.
