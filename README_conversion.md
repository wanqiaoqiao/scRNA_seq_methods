# Convert One Cell Ranger Matrix to Raw Counts CSV

This script converts one 10x Cell Ranger output matrix into a GEO-style raw count CSV file.

## Purpose

Cell Ranger outputs single-cell count data in 10x matrix format:

```text
matrix.mtx.gz
barcodes.tsv.gz
features.tsv.gz
This script reads one sample’s filtered_feature_bc_matrix folder and converts it into a CSV file where:
rows = genes
columns = cells
values = raw UMI counts
