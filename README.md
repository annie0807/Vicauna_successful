# News Event Triggered Knowledge Update

## Preprocessing 
- Run sentence-level difference labeling with `netku_edit.py`

## Model
- Under `util/`.

## Source of our dataset
[Data](https://github.com/hhhuang/NetKu)

## Modified Dataset to fit our task
[Data](https://drive.google.com/drive/folders/1fMz10Dts2pxFp0Hz_-EVYoBJEEZERGsL?usp=sharing)

## Bidirectional Sentence Labeling
![bidirectional_labeling](https://raw.githubusercontent.com/theQuert/NetKu_Processing/main/bi_labeling.png)

## Slides
[Google Slides](https://docs.google.com/presentation/d/1Wku83ckWwYP26hAqMmsWmURScCrNR5B7aWaKZAYEspg/edit?usp=sharing)

## References
#### [A Multi-grained Dataset for News Event Triggered Knowledge Update](https://dl.acm.org/doi/10.1145/3511808.3557537)
#### [PRIMERA: Pyramid-based Masked Sentence Pre-training for Multi-document Summarization](https://github.com/allenai/PRIMER)
#### [NewsEdits: A News Article Revision Dataset and a Document-Level Reasoning Challenge](https://github.com/isi-nlp/NewsEdits)
#### [Updated Headline Generation: Creating Updated Summaries for Evolving News Stories](https://aclanthology.org/2022.acl-long.446)
#### [DYLE: Dynamic Latent Extraction for Abstractive Long-Input Summarization](https://ui.adsabs.harvard.edu/abs/2021arXiv211008168M)
#### [EditEval: An Instruction-Based Benchmark for Text Improvements](https://ui.adsabs.harvard.edu/abs/2022arXiv220913331D)
#### [Attention Temperature Matters in Abstractive Summarization Distillation](https://ui.adsabs.harvard.edu/abs/2021arXiv210603441Z)
#### [Graph-to-Text Generation with Dynamic Structure Pruning](https://ui.adsabs.harvard.edu/abs/2022arXiv220907258L)
#### [Improving Wikipedia Verifiability with AI](https://ui.adsabs.harvard.edu/abs/2022arXiv220706220P)
#### [Efficiently Summarizing Text and Graph Encodings of Multi-Document Clusters](https://aclanthology.org/2021.naacl-main.380)
#### [Leveraging Locality in Abstractive Text Summarization](https://ui.adsabs.harvard.edu/abs/2022arXiv220512476L)

## installation bug
### en_core_web_sm installation error: 
```
pip install spacy
python -m spacy download en_core_web_sm
```
https://newreleases.io/project/github/explosion/spacy-models/release/en_core_web_sm-2.3.1

### files2rouge installation error: 
   ```
   pip install -U git+https://github.com/pltrdy/pyrouge
   git clone https://github.com/pltrdy/files2rouge.git
   cd files2rouge
   python setup_rouge.py
   pip install six
   python setup_rouge.py
   python setup.py install
   ```

### longformer and torch
   install torch first
   ```
   pip install torch==1.13.1+cu117 torchvision==0.14.1+cu117 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cu117
   pip install git+https://github.com/allenai/longformer.git
   ```
