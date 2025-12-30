# Ageas enables time-free cell fate inference across single-cell and spatial multi-omics data
### The manuscript for Ageas is currently in preparation, and the preprint and source code will be released upon reaching a significant milestone.

![workflow](image/workflow.png)

Understanding cell fate decisions is fundamental to developmental biology and disease research. However, experimental lineage tracing requires genetic manipulation and is impractical in many systems. Computational approaches often rely on time-resolved measurements, which single-cell and spatial omics studies rarely provide. Here, we present Ageas, a time-free transfer learning framework for cell fate inference from single-cell and spatial multi-omics data. Ageas overcomes these limitations by learning fate memory from terminal cell populations and transferring this information to progenitor or intermediate cells, enabling fate bias inference from static molecular snapshots. To enable robust generalization across molecular modalities, Ageas employs a data-adaptive ensemble strategy with automated model selection. In benchmark datasets with lineage-traced scRNA-seq and scATAC-seq, as well as spatial transcriptomics data, Ageas achieves strong performance compared to existing methods. Applying Ageas to a 3D human embryo reveals a spatially organized anterior–posterior gradient of epiblast fate priming, with anterior epiblast cells biased toward ectodermal fates and posterior cells toward primitive streak–derived lineages, accompanied by regionally graded fate-associated regulatory programs. Together, these results establish Ageas as a general framework for decoding cell fate relationships from static molecular snapshots.

### Our work introduces a conceptual advance in cell fate inference and provides several key contributions:

-**Time-Free Fate Inference through Transfer Learning**: Ageas reframes lineage prediction as a transfer of information from terminal cell states to their progenitors, eliminating the need for time-series or experimental lineage tracing. This approach allows cell fate bias to be decoded directly from a single snapshot of molecular data, opening new avenues to study developmental processes that cannot be sampled over time (such as human embryogenesis or clinical samples).

-**General and Modality-Agnostic Framework**: Ageas generalizes across transcriptomic, epigenomic, and spatial modalities via a data-adaptive ensemble strategy. Using multiple lineage-tracing benchmarks with ground-truth fate outcomes, Ageas consistently outperforms existing state-of-the-art methods in predicting progenitor fate bias across diverse biological systems.

-**Spatially Organized Fate Priming in the Human Epiblast**: Lineage-tracing studies in mouse embryos have revealed biased contributions of epiblast cells to downstream lineages, but offer limited insight into the origins of this bias. In human embryos, epiblast fate bias remains unknown, as genetic lineage tracing is not feasible. By applying Ageas to a 3D human embryo spatial atlas, we demonstrate that human epiblasts similarly exhibit fate bias toward distinct downstream lineages and provide a spatial interpretation of this bias.

-**Model-Based Interpretation of Fate-Associated Regulatory Programs**: Ageas identifies lineage-driving regulators through an interpretable explanation module and enables virtual cell–based in silico perturbation, providing a computational foundation for virtual cell analyses of fate decisions.



### Apply Ageas on scRNA-seq data

[Predict progenitor fate bias for IEP reprogramming](https://jiang-junyao.github.io/AEGAS_analysis/scRNA_reprogramming)

### Apply Ageas on spatial transcriptome

[Predict epiblast fate bias during human Embryogenesis](https://jiang-junyao.github.io/AEGAS_analysis/3D_human_embryo)