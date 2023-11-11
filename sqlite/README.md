# About

This is showcase how to turn those CSV files into SQLite database.

`cyberincidents.db` is SQLite DB with all CSV imported as tables.

## How to import EuRepoC CSV to SQLite

1. Install [sqlite-utils](https://sqlite-utils.datasette.io/)
    ```shell
    pip install sqlite-utils
    ```
2. Import CSVs to DB
    ```shell
    sqlite-utils insert cyberincidents.db incidents ../data/EuRepoC_Global_Database_1.1.csv --csv --encoding=UTF-8
    sqlite-utils insert cyberincidents.db attribution ../data/EuRepoC_Attribution_dataset_1.1.csv --csv --encoding=UTF-8
    sqlite-utils insert cyberincidents.db receiver ../data/EuRepoC_Receiver_dataset_1.1.csv --csv --encoding=UTF-8
    ```

