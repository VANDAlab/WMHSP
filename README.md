# WMHSP

Neurodegenerative diseases such as Alzheimer’s disease (AD) commonly coexist with cerebrovascular disease in the elderly population. Cerebral small vessel disease (SVD) is the most common vascular cause of dementia and a major contributor to mixed dementia. SVD frequently coexists with AD and can increase the cognitive and physical deficits caused by neurodegeneration. White matter hyperintensities (WMHs) are considered to be one of the major signs of SVD on MRI and are associated with neurological and cognitive symptoms and physical difficulties. We have developed automated tools for segmentation of WMHs in Alzheimer’s patients using multiple contrasts of MR images. We use these segmentations to study the effect of WMHs in AD.

This version of the pipeline is also available [here](https://nist.mni.mcgill.ca/white-matter-hyperintensities/)

## Execution:

python ./WMHSP.py -c RF -i training_inputs.csv -d N -m template_mask.mnc -f 10 -o outputs/ -t Temp_Files/ -e PT -n segmentation_inputs.csv -p Trained_Classifiers/

## Input csv format:
Subjects,T1s,FLAIRs,Masks,XFMs 
S1,t1.mnc,flair.mnc,mask.mnc,xfm.xfm

## References: 

- Dadar, M., Maranzano, J.,…, Collins, D.L. & Alzheimer’s Disease Neuroimaging Initiative. (2017). Performance comparison of 10 different classification techniques in segmenting white matter hyperintensities in aging. NeuroImage, 157, 233-249.
- Dadar, M., Maranzano, J., Ducharme, S., Carmichael, O. T., Decarli, C., Collins, D. L., & Alzheimer’s Disease Neuroimaging Initiative. (2018). Validation of T 1w‐based segmentations of white matter hyperintensity volumes in large‐scale datasets of aging. Human brain mapping, 39(3), 1093-1107.
 
