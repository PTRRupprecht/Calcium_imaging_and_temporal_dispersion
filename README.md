## Calcium imaging and temporal dispersion

Analysis of temporal dispersion from calcium imaging data processed with a spike inference algorithm

### Getting started

To get started, just [open this Colab Notebook](https://colab.research.google.com/github/PTRRupprecht/Calcium_imaging_and_temporal_dispersion/blob/main/Temporal_dispersion_of_activity_from_deconvolved_calcium_imaging.ipynb).

### Background

Calcium imaging is temporally less precise than electrophysiology. [A recent study by Wei et al. (2020)](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008198) showed that under the investigated imaging conditions, neuronal activity that appeared to have more or less clearly defined bouts from electrophysiological recordings appeared to be more continuous (like a smooth sequence) from calcium imaging data, even if those were deconvolved.

Is this indeed not possible to clearly distinguish smooth sequential activity patterns from more discrete bouts using calcium imaging? The short answer is, no; it is possible, under certain conditions.

I have described my approach to this question on this blog post. This Colaboratory Notebook is just a supplementary material to [this blog post](https://gcamp6f.com/2021/02/23/temporal-dispersion-of-spike-rates-from-deconvolved-calcium-imaging-data-with-cascade/), allowing any interested reader to replicate the analysis and to add their own analysis.

Briefly, the Notebook downloads the [Cascade](https://github.com/HelmchenLabSoftware/Cascade) toolbox into the Cloud-based environment, loads an appropriate global model see the [preprint](https://www.biorxiv.org/content/10.1101/2020.08.31.272450v2), Fig. 3, for a description of this global model), uses one of the ground truth datasets to generate ground truth at a given noise level and then evaluates the dispersion of inferred spike rates in comparison to the ground truth.
