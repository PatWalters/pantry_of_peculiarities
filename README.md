# Pat's Cabinet of Curiosities
Questions regarding ML in drug discovery that keep me up at night.  Please submit an issue or PR to comment, add to, or change this list.

### Molecular Representation
- Are learned representations better? How can we prove it?
- Do foundation models improve predictive performance?
- If we're training foundation models on data derived from molecular graphs (e.g., Mordred descriptors), can we expect them to generalize?
- As chemists, we know that benzene and thiophene are isosteric and similar, so why don't our molecular representations capture this?
- How can we incorporate conformational flexibility into a molecular representation (i.e., how do we handle multiple conformers in ML)?
- Is there a case in the literature where a 3D QSAR method has outperformed 2D?

### Defining a model’s applicability domain
- Can we improve on the similarity to the training set when determining model applicability?
- Can model uncertainty help us understand where a model will perform poorly?

### Global vs local models 
- Do local models really outperform global models?  How can we test this? 

### Multi-task models 
- How closely related to tasks do they have to be for multitasking to be effective?
- Can multitasking make models worse?

### Foundation models and fine-tuning
- What is the impact of dataset size on foundation model performance?
- What is the impact of dataset composition on foundation model performance?

### Model interpretability
- How do we get to models that can provide guidance on what to make next? 

### Quantifying uncertainty 
- Are ensembles the best way to quantify uncertainty?
- Are Gaussian processes better than ensembles for assessing uncertainty?
- Can we use the submissions to the Expansion challenge to assess which compounds were consistently mispredicted? Could we have anticipated these failures?
- Key references
    - https://doi.org/10.1021/acs.jcim.5c02381

### Structure prediction (co-folding) 
- Can we anticipate when co-folding will work?
- Can we get accurate poses from Boltz-2 or OF-3?
- Can we get accurate affinities from co-folding methods?

### Data 
- How do we handle truncated data (e.g “>40”)
- Key references
    - https://doi.org/10.1016/j.ailsci.2025.100128

### Multi-objective optimization
- How can we simultaneously optimize compounds for multiple criteria
- Key references
    - https://www.sciencedirect.com/science/article/pii/S2666389923000016

### Benchmark Realism & Validation
- Do standard benchmarks (e.g., MoleculeNet) actually reflect real-world drug discovery challenges like time-based splits or structural novelty?
- How can we develop metrics that correlate better with success in the "wet lab" than simple ROC-AUC or RMSE?
- Key references
    - https://polaris-hub.github.io/polaris-catalog/ (Polaris)

### Data Quality & Experimental Bias
- How much of our model performance is derived from memorizing experimental noise or artifacts in public datasets?
- How do we handle "publication bias" (the missing negative results) when training on literature-mined data?
- Can we reliably integrate data across different labs and assays (the "batch effect" problem)?
- Key references
    - https://doi.org/10.1021/acs.jcim.9b01075 (In Need of Bias Control)
    - https://doi.org/10.1038/s41592-021-01205-4 (DOME recommendations)

### Active Learning & Experimental Design
- What is the optimal strategy for balancing exploration (sampling new chemical space) vs. exploitation (optimizing a lead series)?
- How do we choose the most "informative" compounds to synthesize when resources are limited to 10–20 molecules per cycle?
- Key references
    - https://doi.org/10.1002/minf.201400153 (Active-learning strategies)

### Synthesis & Feasibility
- How do we incorporate "synthesizability" into generative models without restricting them to trivial chemistry?
- Can ML accurately predict reaction yields and purification difficulty, or just "if" a reaction works?
- Key references
    - https://doi.org/10.1021/acs.accounts.8b00462 (Computer-Aided Synthesis Planning)

### Bridging Physics and ML
- How can we use ML to accelerate physics-based simulations (e.g., MD, QM) without losing their fundamental accuracy?
- Do hybrid models (ML + Physics) generalize better to novel scaffolds than pure ML models?
- Key references
    - https://doi.org/10.1039/D1SC06578C (PIGNet)

### Biology & Systems Complexity
- Can we transition from predicting "binding to a protein" to predicting "cellular or organism-level effects"?
- How do we model "polypharmacology" (multi-target effects) to predict both efficacy and off-target toxicity?
- Key references
    - https://doi.org/10.1038/s41587-023-01784-y (Foundation models for biology)

### Low-Data Regimes (SAR-lite)
- How can we build useful models when we only have 5–10 data points at the start of a project?
- Are transfer learning or few-shot learning techniques actually effective in these "SAR-lite" scenarios?
- Key references
    - https://doi.org/10.48550/arXiv.2104.10681 (FS-Mol)
    - https://doi.org/10.1039/D4SC05204F (MHNfs)

