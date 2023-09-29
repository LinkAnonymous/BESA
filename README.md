# BESA

This repository contains code to reproduce the key results of the paper BESA: Pruning Large Language Models with Blockwise Parameter-Efficient Sparsity Allocation.

## Dependencies

* `torch`: tested on v2.0.1+cu118
* `transformers`: tested on v4.31.0
* `accelerate`: tested on v0.21.0
* `datasets`: tested on v2.14.4
* `timm`: tested on v0.9.5

**lm-evaluation-harness**
```
git clone https://github.com/EleutherAI/lm-evaluation-harness
cd lm-evaluation-harness
pip install -e .
```

**Customized Cuda Operator**
```
cd models/ops
python setup.py install
```

## Usage

Here is the command to run baseline experiments followed by perplexity evaluations on WikiText2, PTB, C4 and zero-shot tasks.
See also the CMD-argument documentation.

```
bash main_exps.sh
```
