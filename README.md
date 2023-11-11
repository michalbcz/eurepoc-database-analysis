# About

This project is showcase of several data analysis methods.

For that we are using [EuRepoC database](https://eurepoc.eu/database/).

The European Repository of Cyber Incidents (EuRepoC) is an independent research consortium dedicated to better understanding the cyber threat environment in the European Union and beyond. 

## Data

All the data are downloaded in `/data` directory.

### Re-download data when needed

1. CSV files:
```shell
curl -O --create-dir --output-dir ./data "https://zenodo.org/records/7848941/files/EuRepoC_Global_Database_1.1.csv?download=1" 
curl -O --create-dir --output-dir ./data "https://zenodo.org/records/7848941/files/EuRepoC_Attribution_dataset_1.1.csv?download=1"
curl -O --create-dir --output-dir ./data "https://zenodo.org/records/7848941/files/EuRepoC_Receiver_dataset_1.1.csv?download=1"
```
2. Excel file (for Excel based analysis): 
```shell
curl -O --create-dir --output-dir ./data "https://zenodo.org/records/7848941/files/EuRepoC_Global_Database_1.1.xlsx?download=1"
```

## Sub-projects

/jupyter ([Jupyter notebooks](https://jupyter.org/))
    - [Worldcloud from name and description](./jupyter/cyberincidents_word_cloud.ipynb)