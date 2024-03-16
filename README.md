# Nature - Disappearing Cities On US Coasts

This repository contains the Python code and instructions necessary to replicate the analysis presented in the "Disappearing cities on US coasts" paper using the Osyris Replicate python package. The analysis focuses on the combined effects of projected sea-level rise and coastal land subsidence on future flooding risks in major US cities.

## Steps to Replicate the Analysis

### Getting started
Install and import the package

`pip install osreplicate`\
`from osreplicate import Paper`

### Access the paper you want to replicate
Provide the papers alias to start analyzing

`analysis = Paper('nature/Disappearing Cities On US Coasts')`

### Get the datasets
Locally download any available datasets associated with this paper

`analysis.get_data()`

### Replicate the paper
Automatically run the full analysis on the available datasets and reproduce the figures from the paper

`analysis.run()`

### Mix and match      
Access core analysis methods from to the paper

`analysis.wavelet_based_insar_analysis(interferograms)`\
`analysis.generate_insar_los_displacements(sar_frames)`\
`analysis.generate_vlm_rate_map(los_velocities, gnss_datasets)`
