## TG-JEBI

This repository contains the source code of the paper "Triplet-driven Generative Joint Extraction for Biomedical Information Using Word-level and Pointer-guided Decoders" submitted to *Engineering Applications of Artificial Intelligence*.

## Requirements

### Packages and Versions:
1) torch>=1.9.0
2) torchvision>=0.10.0
3) torchaudio>=0.9.0
4) numpy>=1.19.0
5) tqdm>=4.60.0
6) recordclass>=0.15.0

You can install the required dependencies via:

```bash
pip install -r requirements.txt
```
## Datasets

The datasets used for experiments in the paper can be downloaded from the following link:

https://drive.google.com/drive/folders/10zlZOq_nA7P-EtIJFQYFjsjiTtvvFhtr?usp=sharing

## How to run

### Word-level Generative Decoding Model

python word_decoder.py gpu_id random_seed source_data_dir target_data_dit train/test

```
python word_decoder.py 0,1,2 1027 DrugProt/data/ DrugProt/data/word_decode_model train
```
```
python word_decoder.py 0,1,2 1027 DrugProt/data/ DrugProt/data/word_decode_model test
```
### Pointer-guided Generative Decoding Model

python ptrnet_decoder.py gpu_id random_seed source_data_dir target_data_dit train/test

```
python ptrnet_decoder.py 0,1,2 1027 DrugProt/data/ DrugProt/data/ptrnet_decode_model train
```
```
python ptrnet_decoder.py 0,1,2 1027 DrugProt/data/ DrugProt/data/ptrnet_decode_model test
```
## Acknowledgments ##

With great respect, we acknowledge the [BioCreative platform](https://biocreative.bioinformatics.udel.edu/) and extend our sincere appreciation to BioCreative [VI](https://biocreative.bioinformatics.udel.edu/tasks/biocreative-vi/track-5/) & [VII](https://biocreative.bioinformatics.udel.edu/tasks/biocreative-vii/track-1/) for generously providing the corpora and experimental data of various works.


## Citation

Coming soon...
