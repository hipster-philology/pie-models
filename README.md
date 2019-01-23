# Pie Models

This repository contains pretrained models for Pie (A Framework for Joint Learning of Sequence Labeling Tasks).

_More on Pie_: 
[https://github.com/emanjavacas/pie](https://github.com/emanjavacas/pie).

## Find a model

Models are arranged by language. **TODO**: add a json documentation file per model.

### German (de)

`german-ren.model.tar`: Lemmatizer pretrained on a subset of the Referenzkorpus Mittelniederdeutsch/Niederrheinisch: https://www.slm.uni-hamburg.de/ren.html

### Spanish (es)

`spanish-AnCora.model.tar`: Lemmatizer pretrained on the AnCora corpus for Spanish (part of the Universal Dependencies)

### Old French (fro)

`french-Geste.model.tar`: Lemmatizer pretrained on the Geste corpus

`fro-poslemmes_cat-lemma-2019_01_22-02_34_11.tar`: lemmatizer and POS-tagger trained on the Geste corpus, and other Old French data from the École des chartes. 
    
    Target task: lemma. 
    Accuracy on test data
      lemma: 0.9383
      pos: 0.9473

`fro-poslemmes_cat-lemma-2019_01_23-00_34_12`: same as the previous one, but using pre-trained word embeddings from a large unlabelled corpus.

    Target task: lemma. 
    Accuracy on test data
      lemma: 0.9409
      pos: 0.9468

`model_fro_poslemmesmorph.tar`: POS-tagger, lemmatizer and morphological analyzer trained on the Geste corpus

### Latin (lat)

`capitula.model.tar`: Lemmatizer pretrained on a non-open source dataset of medieval latin

### Turkish (tur)

`turkish-IMST.model.tar`: Lemmatizer pretrained on the IMST corpus for Turkish (part of the Universal Dependencies)

## Example config file for training a lemmatizer

`lemma.config.json` is an example config file for training a lemmatizer to reasonable good accuracy.

## PIE

#### Installation

For more information check the repo at [](https://www.github.com/emanjavacas/pie), but in short:

```bash
virtualenv env -p python3.7
source env/bin/activate
pip3 install -r requirements.txt
```
