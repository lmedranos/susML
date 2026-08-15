[![paper-link](https://img.shields.io/badge/arXiv-2604.00069-%23B31B1B
)](https://doi.org/10.48550/arXiv.2604.00069)

# Perspective: Towards sustainable exploration of chemical spaces with machine learning

## About
Artificial intelligence is transforming molecular and materials science, but its growing computational and data demands raise critical sustainability challenges. In this Perspective, we examined resource considerations across the AI-driven discovery pipeline, building on discussions from the **SusML workshop: Towards sustainable exploration of chemical spaces with machine learning** held in Dresden, Germany. 

<p align="center">
<img width="600" alt="workflow" src="img/susml.png" />
</p>

## Carbon footprint in the AI-driven discovery pipeline

As part of this perspective, we compiled a table reporting the estimated carbon footprint of representative examples spanning quantum-mechanical datasets generation, machine-learning force fields, large language models, and quantitative structure-property/activity relationship models. Carbon footprints were estimated using the [![link](https://img.shields.io/badge/%F0%9F%8C%B1%20Green%20Algorithm-E8F5E9)](https://calculator.green-algorithms.org/) framework, a web-based initiative that allow researchers to estimate the environmental impact of computational workloads based on parameters such as runtime, number of cores/GPUs used, memory, location, etc.

We invite the community to contribute their own data by adding new entries to this `README` file and submitting a pull request. By collectively reporting computational requirements alongside model performance, we aim to establish a living, community-driven resource for comparing the computational and environmental costs of machine-learning approaches and to encourage more transparent and sustainable computational practices in the field.

### Quantum-Mechanical Dataset Generation

| Name | Description | Computing time [hrs] | Carbon footprint [CO₂e] | Ref. | 
|---|---|---:|---:|---:| 
| QM7-X | $\approx$ 4.2 M small molecules | 3.27 M CPU | 9.14 tons | [Hoja et al. (2021)](https://www.nature.com/articles/s41597-021-00812-2)| 
| ANI-1x/1ccx | $\approx$ 5.5 M small molecules | 14 M CPU | 32.23 tons |
| GEMS | $\approx$ 3 M molecular building blocks and biomolecular fragments | 576 M CPU | 12,800 tons |
| QUED-LD50 | $\approx$ 3.6 M drug-like molecules | 314 k CPU | 1.34 tons |
| OMol25 | $\approx$ 140 M diverse molecular systems | 6.6 B CPU | 20,600 tons |
| Materials Project | $\approx$ 785 k materials and molecules | 965 M CPU | 18,900 tons |
| OMat24 | $\approx$ 118 M materials | 400 M CPU | 1,250 tons |
| MAD-1.5 | $\approx$ 216 k materials and molecules | 40 M CPU | 30 tons |
| **+ Add entry** |  |  |  |

### General-Purpose Machine Learning Interatomic Portentials

#### (Bio)molecular simulations
Equivariant models trained on molecular QM data for (bio) molecular simulations

| Name | Description | Computing time [hrs] | Carbon footprint [CO₂e] | 
|---|---|---:|---:|
| MACE-OFF23(L) |  | 336 GPU | 28.34 kg |
| MACE-POLAR1(M) |  | 15,360 GPU | 2.75 tons |
| MACE-POLAR1(L) |  | 23,040 GPU | 4.13 tons |
| SO3LR |  | 86 GPU | 12.81 kg |
| **+ Add entry** |  |  |  |

#### Materials
Equivariant models trained on materials QM data for materials simulations

| Name | Description | Computing time [hrs] | Carbon footprint [CO₂e] | 
|---|---|---:|---:|
| MACE-MP-0 |  | 2,600 GPU | 236.62 kg |
| GRACE-1L-OMAT |  | 400 GPU | 73.67 kg |
| GRACE-2L-OMAT-L |  | 700 GPU | 128.92 kg |
| PET-MAD-XS |  | 143 GPU | 5 kg |
| PET-MAD-S |  | 190 GPU | 7.5 kg |
| **+ Add entry** |  |  |  |

### Large Language Models

| Name | Description | Computing time [hrs] | Carbon footprint [CO₂e] | 
|---|---|---:|---:|
| BERT | GP bidirectional transformer language model | - | 652 kg |
| BERT-QA | Fine-tuned for extractive question-answering tasks | - | 46.4 g |
| MechBERT Cased | Pretrained on MechEng literature | 600 GPU | 188.77 kg |
| BERT-MechQA | Fined-tuned for | < 4 GPU | 1.26 kg |
| XLNet-MechQA | MechEng question-answering | < 4 GPU | 1.26 kg |
| Llama-MechQA | tasks | 16 GPU | 5.03 kg |
| Llama 3.1-405B | Meta GP-LLM with 405B and | 30.84 M GPU | 8,930 tons |
| Llama 3.1-70B | 70B parameters | 7M GPU | 2,040 tons |
| Olmo 3-32B | AI2 GP-LLM with 32B and | 1.12 M GPU | 502,871 tons |
| Olmo 3-7B | 7B parameters | 246.5 k GPU | 104,701 tons |
| **+ Add entry** |  |  |  |

### Quantitative Structure-Property Relationships

| Name | Description | Computing time [hrs] | Carbon footprint [CO₂e] | 
|---|---|---:|---:|
| SISSO(10F) | - | - | 8.18 g | 
| SISSO(50F) | - | - | 492.42 g | 
| ENINet | Regression model trained | 6.5 GPU | 1.27 kg | 
| SchNet | on QM9 dataset | 21 GPU | 4.79 kg | 
| QUED-D$_\text{QM}$ | Regression model trained | 14.9 CPU | 89 g | 
| QUED-SOAP | on QUED-LD50 dataset | 7.16 k CPU | 33.86 kg | 
| **+ Add entry** |  |  |  |
