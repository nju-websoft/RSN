## RSN

Lingbing Guo, Zequn Sun, Wei Hu*. [Learning to Exploit Long-term Relational Dependencies in Knowledge Graphs](https://arxiv.org/abs/1905.04914). In: _ICML_ 2019

## INSTALLATION

1. Please first install Python 3.5+, and then unpack data.7z.

2. Type <code>pip install -r requirements</code> in shell to install required packages. Note that, when using Tensorflow 1.2+, the learning rate has to be re-adjusted. We suggest using tensorflow-gpu = 1.1.

## RUNNING

1. Run jupyter by typing <code>jupyter notebook</code> in shell.

2. In the opened browser, click RSN4EA.ipynb for entity alignment, or RSN4KGC.ipynb for KG completion.

3. The files RSN4EA.ipynb and RSN4KGC.ipynb record the latest results on DBP-WD (normal) and FB15K, respectively.

4. You can also click 'Toolbar -> Kernel -> Restart&Run All' to run these two experiments.


## DATA

1. Limited by the space, we only uploaded FB15K for KG completion. For WN18 and FB15K-237, you can easily download them from the Internet.

2. Change options.data_path or other options.* to run RSN on different datasets with different settings.

3. For RSN4KGC.ipynb, we adopt a matrix filter method for evaluation, which may use more than 64GB memory.

4. For entity alignment, V1 denotes the normal datasets, and V2 denotes the dense ones. Please use first 10% data of <code> ref_ent_ids</code> for validation.

5. entity-alignment-full-data.7z provides a complete version of the EA datasets, including attribute files and datasets with different proportions. 

## CITATION

If you find our work useful, please kindly cite it as follows:

```
@inproceedings{RSN,
  author    = {Lingbing Guo and Zequn Sun and Wei Hu},
  title     = {Learning to Exploit Long-term Relational Dependencies in Knowledge Graphs},
  booktitle = {ICML},
  pages     = {2505--2514},
  year      = {2019}
}
```
