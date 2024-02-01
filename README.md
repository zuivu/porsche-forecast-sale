# BIS Group 6 - Submission

The structure of this folder:

### scripts:
- model.ipynb: our current notebook with our meta model
- features_final_v2.ipynb: our feature preperation pipeline

### output_data:
- 2 runs of output data
- each run contains:
    - a list with columns that have NaN values for the future
    - a list with columns that have predictions instead of NaN values for the future
    - the preprocessed datalist (with columns created by our 5 methods)
    - the feature importance list with is created via shap
    - the feature importance list created via .corr()

### data:
- the input data

### archive:
- old but still interesting code

### and our predictions plus two result charts