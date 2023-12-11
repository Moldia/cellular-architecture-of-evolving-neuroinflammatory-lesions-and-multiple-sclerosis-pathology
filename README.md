# dynamics-of-multiple-sclerosis-lesion-and-disease-evolution
## abstract
Multiple sclerosis (MS) is a neurological disease characterized by multifocal lesions and smoldering pathology. While single-cell analyses provided insights into cytopathology, evolving cellular processes underlying MS remain poorly understood. We modeled the cellular dynamics of MS by examining temporal and regional rates of disease progression in mouse experimental autoimmune encephalomyelitis. By performing single-cell spatial expression profiling using In situ sequencing, we annotated disease neighborhoods during lesion evolution and found centrifugal propagation of active lesions. We demonstrated that disease-associated (DA)-glia arise independently of lesions and are dynamically induced and resolved over the disease course. Single-cell spatial mapping of human archival MS spinal cords confirmed the differential distribution of homeostatic and DA-glia, enabled deconvolution of active and inactive lesions into sub-compartments, and identified new lesion areas. By establishing a spatial resource of mouse and human MS neuropathology at a single-cell resolution, our study unveils the intricate cellular dynamics underlying MS evolution.

## breakdown
### processing code
code used process the data from the iss and xenium experiments, which includes image restoration (CARE; for the iss data), preprocessing, decoding and postprocessing. the postprocessing includes the cell segmentation and the creation of the adata objects that were used downstream for cell type clustering and annotation. 

### visualization code
code used to generate the figures in the paper.

Correspondence: christoffer.langseth@scilifelab.se, petra.kukanja@ki.se, mats.nilsson@scilifelab.se, goncalo.castelo-branco@ki.se 