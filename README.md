# Verified ATL Scheduling Framework

This repository contains the implementation and demonstrations of the verified
ATL user-scheduling framework. It is compatible with Coq 8.13.2.

To build the framework, simply run `make` in the `src` directory.

The C code generated from our set of examples can be found in `src/clib`. It can
also be regenerated by running `make clib` from `src`.

For a set of simple programs and proofs to walk through please see:
* `pipeline_schedule` in `src/Blur.v`. This is a walkthrough of the
scheduling proof for the example in the introduction of our paper.
* `scatter_gather` in `src/GatherScatter.v`. This is a walkthrough of the
scheduling proof for the scatter-to-gather transformation mentioned in the
evaluation section of our paper.
* `equiv` in `src/Im2col.v`. This is a walkthrough of im2col transformation
outlined in the evaluation section of our paper.

For the full-scale proof constructing the tiled blur performance evaluation
example, please see `total_fusion_to_tiled` in `src/Blur.v`.
