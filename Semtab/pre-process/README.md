# Pre-process procedures

## Start from scratch:

1. First run [transform_to_json.py](https://github.com/RECA-paper/RECA/blob/main/Semtab/pre-process/transform_to_json.py) to transform the raw table input (in csv format) to table summaries (in json format).
2. Then run [NER_extraction.py](https://github.com/RECA-paper/RECA/blob/main/Semtab/pre-process/NER_extraction.py) to extract the named entities from the tables.
3. Run [pre-process.py](https://github.com/RECA-paper/RECA/blob/main/Semtab/pre-process/pre-process.py) to find the related and sub-related tables and perform table alignment.
4. Run [make_json_input.py](https://github.com/RECA-paper/RECA/blob/main/Semtab/pre-process/make_json_input.py) to split the data into train-val and test sets and transform them into jsonl format.
5. Run [jaccard_filterjson.py](https://github.com/RECA-paper/RECA/blob/main/Semtab/pre-process/jaccard_filterjson.py) to apply table filtering.
6. Run [semtab-datasets.py](https://github.com/RECA-paper/RECA/blob/main/Semtab/pre-process/semtab-datasets.py) to generate the tokenized input for RECA.

## Start from pre-processed jsonl data:
1. Download the pre-processed jsonl data, see instructions in [jsonl_data](https://github.com/RECA-paper/RECA/tree/main/Semtab/data/jsonl_data).
2. Run [semtab-datasets.py](https://github.com/RECA-paper/RECA/blob/main/Semtab/pre-process/semtab-datasets.py) to generate the tokenized input for RECA.
