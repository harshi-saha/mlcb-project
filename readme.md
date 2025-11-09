**Reference:**
- Nature Paper: [link](https://www.nature.com/articles/s41592-022-01667-0)
- Nature Paper Git: [link](https://github.com/carpenter-singh-lab/2022_Haghighi_NatureMethods)

**Reference Data Download:**
- Install AWS CLI: [link](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
- Run the below in CLI:
```
aws s3 sync \
  --no-sign-request \
  s3://cellpainting-gallery/cpg0003-rosetta/broad/workspace/preprocessed_data .
```

**Provided Data:** \
The processed data used for this project can be found at [link](https://drive.google.com/file/d/1Mz1VAHP2iBwdJk8uRrFB3UgaBoMnjZFD/view?usp=sharing).
The data provided here are the curated data as processed from the data that can be downloaded via the directions above. 

For each dataset (LINCS, Bray, Caicedo, and Rohban), the processed L1000 assay data (`replicate_level_cp_augmented.parquet`) and cellprofiler data (`replicate_level_l1k.parquet`) are provided. 

The scripts to generate these processed parquet files are in `curate_dataset.ipynb` and `curate_eda.ipynb`, run on the data from the AWS bucket in that order. 


