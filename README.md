# Causal_Inference_Anticonflict

Due to the large size of the dataset, we don't include the data file into the repo. To run this project, you need to put your csv data file under /data directory and run the Python Notebook.

The original dataset can be find at https://www.icpsr.umich.edu/web/civicleads/studies/37070/datadocumentation

## School Level Causal Effect Estimation

Run school_level_causal_inference_pipeline.ipynb will return the causal effect estimation between training assignment and anti-conflict score outcome of that school.

## Student Level Causal Effect Estimation

Run student_level_causal_inference_pipeline.ipynb will return the causal effect estimation between training attendance and anti-conflict score outcome of the student. The interference effect due to the student social network has already been considered in the estimation.

## Social Network Interference Mining

To understand how the 'network_effect' comes in the final dataset, please run the network_analysis.ipynb file to go through the process of building social network graphs for each school and use multiple minimum distance graph algorithm to find out the number of trained friends in every student's 1-jump and 2-jump network.

