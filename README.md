# Spatial and cellular dynamics of multiple sclerosis disease evolution and neuropathology in mouse and human 
This repository contains the notebooks used to generate the data and the figures in the preprint: https://www.biorxiv.org/content/10.1101/2023.06.29.547074v1
## Experimental set up
We collected tissues from mice injected with MOG35-55, which triggers myelin-specific T cells to progressively infiltrate the spinal cord in an ascending manner. Tissues were collected at peak from the lumbar region of the spinal cord and more cranial regions of the spinal cord (thoracic and cervical) and the brain. Addutionally, we collected lumbar sections from non-sympotomatic mice and at symptom onset as well as late stage lumbar and cervical sections. To correlate these findings with human spinal cord pathology in MS patients, we applied ISS with the [Xenium In situ platform](https://www.10xgenomics.com/platforms/xenium?utm_medium=search&utm_source=google&utm_campaign=sem-goog-2022-website-page-ra_g-p_xenium-nonbrand-emea&useroffertype=quote-request&userresearcharea=ra_g&userregion=emea&userrecipient=customer&usercampaignid=7011P0000013tOuQAI&gad_source=1&gclid=CjwKCAiApuCrBhAuEiwA8VJ6JnwJuWTlH9H7mh4igrtw9IG59swRfolzDz0Qo-w7TjvLjOOFj-5WWRoCv6cQAvD_BwE) to six human post-mortem cervical spinal cord cross-sections, two control (CTRL1 and CTRL2) and four progressive MS samples bearing pathologically annotated active (MSa1 and MSa2) or inactive lesions (MSi1 and MSi2). 

![EAE schema](images/eae_schema.png)

## Abstract
Multiple sclerosis (MS) is a neurological disease characterized by multifocal lesions and smoldering pathology. While single-cell analyses provided insights into cytopathology, evolving cellular processes underlying MS remain poorly understood. We modeled the cellular dynamics of MS by examining temporal and regional rates of disease progression in mouse experimental autoimmune encephalomyelitis. By performing single-cell spatial expression profiling using In situ sequencing, we annotated disease neighborhoods during lesion evolution and found centrifugal propagation of active lesions. We demonstrated that disease-associated (DA)-glia arise independently of lesions and are dynamically induced and resolved over the disease course. Single-cell spatial mapping of human archival MS spinal cords confirmed the differential distribution of homeostatic and DA-glia, enabled deconvolution of active and inactive lesions into sub-compartments, and identified new lesion areas. By establishing a spatial resource of mouse and human MS neuropathology at a single-cell resolution, our study unveils the intricate cellular dynamics underlying MS evolution.
![Fig1](images/Fig1.png)
(A) UMAP depicting cell populations of EAE and control spinal cord and brain sections. Labels on the UMAP correspond to the 23 main annotated cell types, which were further subclustered into 41 fine clusters. (B) A heatmap with selected differentially expressed genes across main cell types. Shown is the mean z-score. (C) Representative cell maps (see legend in A) across EAE time points and caudal-to-cranial CNS regions. Scale bars – 325μm. (D) Zoom-ins of insets annotated in C. Inset size - 325μm. (E) Strip plot showing the distance from tissue boundary (meninges) of DC, MC/d, and T-cell populations. (F) Numbers of DC, MC/d, and T-cell populations normalized by tissue area across EAE timepoints and spinal cord regions.  

### Centrifugal lesion propagation model
![centrifugal model](images/centrifugal_model.png)
## Code description
For a complete breakdown of the code used to generate the *in situ* sequencing data for the mouse, please visit: https://github.com/Moldia/Lee_2023 or the following repos for CARE: https://github.com/Moldia/ISS_CARE, for preprocessing: https://github.com/Moldia/ISS_preprocessing, for decoding: https://github.com/Moldia/ISS_decoding and for postprocessing: https://github.com/Moldia/ISS_postprocessing. For insights into the best working practises for treating xenium data please visit: https://github.com/Moldia/Xenium_benchmarking. 

### Processing code
Notebooks used to process the data from the ISS and Xenium experiments, which includes image restoration (CARE; for the ISS data), preprocessing, decoding, and postprocessing. The postprocessing includes the cell segmentation and the creation of the adata objects that were used downstream for cell type clustering and annotation. These notebooks are supplied for transparency, and we cannot guarantee that they will work flawlessly for you. If you need help in setting up the environment and running the notebooks, please read the manual supplied here: https://github.com/Moldia/Lee_2023/blob/main/ISS_manual_Supplementary_dRNA.pdf. 


### Visualization code
Notebooks used to generate the figures in the paper.

## Data and code availability 
The ISS data from the 52 mouse samples and the 6 human MS samples are deposited at Zenodo under the DOI: 10.5281/zenodo.8037425. The data is available in one anndata format, compatible with scanpy and squidpy. The data can be explored further at https://tissuumaps.scilifelab.se/2023_spinal_brain.html. 

## Keywords
Spatial sequencing, multiple sclerosis, neuroinflammation, disease-associated glia


Contact: christoffer.langseth@scilifelab.se
