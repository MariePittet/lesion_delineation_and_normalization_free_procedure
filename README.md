# lesion_delineation_and_normalization_free_procedure
Lesion delineation and normalization using a free procedure (+ advices for TBI lesion delineation).

You'll need to have a linux terminal such as WSL on Windows. Sometimes, there are just too many compatibility issues between ITK-SNAP lesion masks and normalization scripts in FSL (even after reorienting, resampling, etc), and you may have to resort to using SPM on Matlab.
In any case, always check your normalized lesions!!!

For questions: [marie.pittet93@gmail.com](mailto:marie.pittet93@gmail.com)


## Lesion delineation:
I used the free software [ITK-Snap](https://www.itksnap.org/pmwiki/pmwiki.php) which allows to view and draw lesions on multiple scanning modalities all at once.

## Lesion normalization:
Free bash pipeline using FSL. Input: your binary lesion masks. Output: normalized binary lesion masks (brought to MNI 152 space)
- Upgrades WSL if needed
- Converts DICOM to Nifti
- Reorients the files
- Normalizes the lesion masks

