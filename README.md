# RECA
This is the repository for the code and data of paper: RECA: Related Tables Enhanced Column Semantic Type Annotation Framework.


![Overview of RECA](./imgs/pipeline_updated.drawio.png)

## Install

```console
$ git clone [link to repo]
$ cd RECA
$ pip install -r requirements.txt 
```

## Reproduce the results

In order to reproduce the results on Semtab2019 dataset, please go through the following steps:
1. Remove the init files in all the directories (they are created for placeholding purpose on github).
2. Download the pre-trained models and pre-processed data, please check the instructions in [checkpoints](https://github.com/RECA-paper/RECA/tree/main/Semtab/checkpoints) and [jsonl_data](https://github.com/RECA-paper/RECA/tree/main/Semtab/data/jsonl_data) for details. 
3. Tokenize the jsonl data, please follow the suggestions in [pre-process](https://github.com/RECA-paper/RECA/tree/main/Semtab/pre-process) (Alternatively, you can download the raw dataset from [here](http://www.cs.ox.ac.uk/isg/challenges/sem-tab/2019/#datasets) and pre-process the data from scratch. For detailed instructions please check [pre-process](https://github.com/RECA-paper/RECA/tree/main/Semtab/pre-process)).
4. Run the experiments, you can either load the pre-trained models and run [RECA-semtab-test-from-pre-trained.py](https://github.com/RECA-paper/RECA/blob/main/Semtab/experiment/RECA-semtab-test-from-pre-trained.py) or train from scratch by running [RECA-semtab-train+test.py](https://github.com/RECA-paper/RECA/blob/main/Semtab/experiment/RECA-semtab-train%2Btest.py)

In order to reproduce the results on WebTables dataset, please go through the following steps:
1. Remove the init files in all the directories (they are created for placeholding purpose on github).
2. Download the tokenized data or raw dataset, please check the instructions in [pre-process](https://github.com/RECA-paper/RECA/tree/main/Semtab/pre-process).
3. Pre-process the raw dataset, please follow the steps described in 'Start from scrtach' in [pre-process](https://github.com/RECA-paper/RECA/tree/main/Semtab/pre-process).
4. Run the experiment file [RECA-webtables-train.py](https://github.com/RECA-paper/RECA/blob/main/WebTables/experiment/RECA-webtables-train.py) in the [experiment](https://github.com/RECA-paper/RECA/tree/main/WebTables/experiment) folder to start training.
