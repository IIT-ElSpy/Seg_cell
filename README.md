# Seg_cell – Automated Analysis of `.lif` Cell Images

**Seg_cell** is a Python script designed to automatically extract and analyse, both accurately and efficiently, all cell images contained within a `.lif` (Leica Image File). The aim of the code is to create a pipeline that optimises and enhances the workflow for the analysis of biological tissues, particularly cells.

### Features

- Allows the user to select any `.lif` file from which all contained images are automatically extracted.
- Provides two resolution options:
  - **Original resolution** (typically 2048×2048 pixels)
  - **Downsampled resolution** (512×512 pixels) for faster processing at the cost of lower image quality.

### Workflow

1. **Brightness Adjustment**  
   A brief automatic adjustment of image brightness is applied.

2. **Image Selection**  
   Users are prompted to choose whether to:
   - Analyse **all** images in the `.lif` file, or  
   - Analyse **only selected** images.

3. **Cell Detection and Output Generation**  
   For each processed image, the following outputs are generated:
   - A `.png` image showing only the detected cells
   - A `.png` image of the original with an overlaid cell mask
   - The total number of cells counted

4. **Data Export**  
   All results are saved in a `.csv` file, enabling quick and efficient downstream data analysis.

To cite this work, you can use: https://doi.org/10.5281/zenodo.15355995
---


