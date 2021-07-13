# compgen2021Capstone



## Data
### gex.tsv:
        info: gene expression measurements
        shape: fat
        values: log10 FPKM + 0.01

### cnv.tsv:
        info: copy number variation estimations
        shape: fat
        values: binarized

### mut.tsv:
        info: mutation data
        shape: tall
        sample_column_name: sample_id
        feature_column_names:
                - Feature
                - protein_change

### drug_response.tsv:
        info: drug response data
        shape: tall
        values: AUC
