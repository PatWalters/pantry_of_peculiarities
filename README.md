# Pat's Cabinet of Curiosities
Questions regarding ML in drug discovery that keep me up at night

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

