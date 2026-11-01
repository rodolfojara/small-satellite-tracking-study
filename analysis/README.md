# Exploratory analysis

This directory contains the author's exploratory analysis from a research practice related to small-satellite tracking.

## Notebook

- [`coordinate-matching-exploration.ipynb`](coordinate-matching-exploration.ipynb): reads and plots two sample star lists, then applies a recorded affine coordinate transformation to one list for visual comparison.

The sample files are part of the third-party MATCH distribution and are located in `../third_party/MATCH/testdata/`.

A static rendering of the plot is available at [`../docs/images/star-list-coordinate-comparison.svg`](../docs/images/star-list-coordinate-comparison.svg) and is also shown in the main README.

## Transformation coefficients

The six affine-transformation coefficients are preserved as recorded values from the original experiment. Their derivation or fitting procedure is not documented here, and the notebook does not calculate them from the sample catalogs. They should therefore be understood as historical inputs to the visualization, not as a reproduced or independently validated result.

## Dependencies and limitations

The notebook uses Python, Matplotlib, and Astropy (`astropy.io.ascii`). It is a historical exploratory notebook, not a complete star-tracker implementation. Its sample catalogs are MATCH test fixtures, not measurements collected by the author. The notebook does not derive spacecraft attitude or position from tracker measurements.
