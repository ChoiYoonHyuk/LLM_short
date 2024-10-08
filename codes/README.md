## [CIKM '24 - Short] Improving the Text Convolution Mechanism with Large Language Model for Review-Based Recommendation

### Project Structure

```
.
├── README.md
├── requirements.txt
└── Baselines
    ├── HEAD
    ├── SER
    ├── CATN
    └── RCDFM
```

### Setup

- Setup Conda, PyTorch, CUDA
  - > pip install -r requirements.txt
- Download Pretrained Word Embeddings; GloVe (below)
  - https://nlp.stanford.edu/data/glove.6B.zip
  - Place under `'./resources/glove.6B/glove.6B.100d.txt'`
- or Poincare GloVe (below)
  - https://polybox.ethz.ch/index.php/s/TzX6cXGqCX5KvAn/
  - Place under `'./resources/glove.6B/poincare_glove_100D_cosh-dist-sq.txt'`
- Source & Target domain dataset
  - can be excuted with additional downloads: `http://jmcauley.ucsd.edu/data/amazon/`
  - substitute
    - `Toys_and_Games.json`
    - `Video_Games.json`

### Usage

```bash
python3 ./baseline_method/main.py  # Training / Test with following code
```

### Experiments

- The NDCG@10 of validation / testing score will be updated at `./results/`
- Iteration will be 300 epochs
- For this version, we remove early stopping to show the overall scores

### Citation

```
N/A
```
