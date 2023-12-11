# Spatial and cellular dynamics of multiple sclerosis disease evolution and neuropathology in mouse and human 
This repository contains the notebooks used to generate the data and the figures in the preprint: https://www.biorxiv.org/content/10.1101/2023.06.29.547074v1
![EAE schema](images/EAE_schema.png)

## Abstract
Multiple sclerosis (MS) is a neurological disease characterized by multifocal lesions and smoldering pathology. While single-cell analyses provided insights into cytopathology, evolving cellular processes underlying MS remain poorly understood. We modeled the cellular dynamics of MS by examining temporal and regional rates of disease progression in mouse experimental autoimmune encephalomyelitis. By performing single-cell spatial expression profiling using In situ sequencing, we annotated disease neighborhoods during lesion evolution and found centrifugal propagation of active lesions. We demonstrated that disease-associated (DA)-glia arise independently of lesions and are dynamically induced and resolved over the disease course. Single-cell spatial mapping of human archival MS spinal cords confirmed the differential distribution of homeostatic and DA-glia, enabled deconvolution of active and inactive lesions into sub-compartments, and identified new lesion areas. By establishing a spatial resource of mouse and human MS neuropathology at a single-cell resolution, our study unveils the intricate cellular dynamics underlying MS evolution.

## Code description
For a complete breakdown of the code used to generate the *in situ* sequencing data for the mouse, please visit: https://github.com/Moldia/Lee_2023 or the following repos for CARE: https://github.com/Moldia/ISS_CARE, for preprocessing: https://github.com/Moldia/ISS_preprocessing, for decoding: https://github.com/Moldia/ISS_decoding and for postprocessing: https://github.com/Moldia/ISS_postprocessing. For insights into the best working practises for treating xenium data please visit: https://github.com/Moldia/Xenium_benchmarking. 

### Processing code
Notebooks used to process the data from the ISS and Xenium experiments, which includes image restoration (CARE; for the ISS data), preprocessing, decoding, and postprocessing. The postprocessing includes the cell segmentation and the creation of the adata objects that were used downstream for cell type clustering and annotation. These notebooks are supplied for transparency, and we cannot guarantee that they will work flawlessly for you. If you need help in setting up the environment and running the notebooks, please read the manual supplied here: https://github.com/Moldia/Lee_2023/blob/main/ISS_manual_Supplementary_dRNA.pdf. 


### Visualization code
Notebooks used to generate the figures in the paper.

## Keywords
Spatial sequencing, multiple sclerosis, neuroinflammation, disease-associated glia


Contact: christoffer.langseth@scilifelab.se
