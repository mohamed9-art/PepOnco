# PepOnco

PepOnco is a leakage-aware, property-conditional generative framework for ACP-oriented peptide chemical-space modeling and multi-objective candidate prioritization.

The framework was developed using a standardized peptide corpus compiled from dbAMPseq, APD3, CancerPPD2, and DCP. PepOnco uses similarity-aware train-validation-test partitioning, train-supported conditioning, frozen tokenization, conditional sequence generation, memorization auditing, and deterministic multi-objective prioritization.

## Repository contents

- `data/`: processed corpus files and reserved folders for split, conditioning, and tokenization metadata.
- `models/`: trained PepOnco and baseline model checkpoints.
- `results/`: generated candidates, final candidate tables, contextual audit files, and supporting result tables.
- `configs/`: configuration files for training, generation, and prioritization.
- `src/`: source code for preprocessing, model training, generation, benchmarking, auditing, prioritization, and contextual analysis.
- `docs/`: reproducibility notes and manuscript-related documentation.

## Important note

The final peptides reported in this repository are computationally prioritized candidates. They are not experimentally validated anticancer peptides. Experimental assays are required before any claim about anticancer activity, selectivity, toxicity, stability, or therapeutic relevance.

## Data sources

Raw peptide records were compiled from publicly available resources, including dbAMPseq, APD3, CancerPPD2, and DCP. Raw database files are not redistributed here unless allowed by the original data-source terms. Processed and derived files are provided to support reproducibility of the PepOnco analyses.

## Model checkpoints

The `models/` folder includes:

- `cvae_conditional_seed*.pt`: PepOnco conditional CVAE checkpoints.
- `gru_conditional_seed*.pt`: conditional GRU baseline checkpoints.
- `gru_unconditional_seed*.pt`: unconditional GRU baseline checkpoints.
- `vae_unconditional_seed*.pt`: unconditional VAE baseline checkpoints.

## Citation

If you use this repository, please cite the associated PepOnco manuscript.

## Contact

Mohamed Aldaw  
Center of Bioinformatics, College of Life Sciences, Northwest A&F University