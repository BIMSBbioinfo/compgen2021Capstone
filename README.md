# compgen2021Capstone



## Data
The datasets for the course can be accessed here:
```
/data/bimsbstatic/public/akalin/AAkalin_DrugResponse/prepared
```

Every dataset is split into two separate directories:
-      .../all_intersect_genes/
-      .../oncoKB_intersect_genes/
The former contains omic data for all genes shared across datasets and the latter composed of gene present in oncoKB cancer panel.


-----
Subsequently, each folder contains the following data: 


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
