# DeltaQuery

**Paper:** Multi-class 3D point cloud change detection from sparse point labels: DeltaQuery, a handcrafted random forest, and their complement (**in preparation**)

**Datasets:** Urb3DCD-V2, SLPCCD, HKCD and NYC-SCD, released by their authors; they are not redistributed here.

**Code Status:** The code, the label draws and their label counts, the run configurations and the scripts that generate the tables and figures of the paper will be released in this repository.

## Overview

DeltaQuery trains dense multi-class change detection on pairs of 3D point clouds from a fixed set of sparse, uniformly sampled point labels. It extends the multi-scale query of the Semantic Query Network (SQN) from static segmentation to change detection. A Siamese KPConv encoder yields target-state features and source-target feature differences at every level. A query head then interpolates them at any point instead of decoding a dense map, so training reads only the labelled points and inference queries every point.

The paper compares DeltaQuery with a sparse-loss decoder trained on the same labels and with a random forest on handcrafted two-epoch geometry, and it studies the equal-weight average of the two models, DeltaQuery+RF.

## Citation

A BibTeX entry will be added when the paper is available.
