# FOLIO: Natural Language Reasoning with First-Order Logic

[UPDATE]: We are excited to release a new version of FOLIO [here](https://huggingface.co/datasets/yale-nlp/FOLIO) with significant quality improvement and error fixing! 

FOLIO is an expert-written, open-domain, logically complex and diverse dataset for natural language reasoning with first-order logic.

FOLIO is released with our paper: [FOLIO: Natural Language Reasoning with First-Order Logic](https://arxiv.org/pdf/2209.00840.pdf).

- folio-v0.0 with train and validation sets are in the data/v0.0 folder.
- A leaderboard will be releeased soon to obtain your results on the unreleased test set.
- We would like to collect more data from the community! Please submit a pull request if you would like to contribute more data points to FOLIO.

## Data Content and Format
This repo contains the train and validation sets in the format of jsonl and txt. Each line in a file contains one example consisting of the following fields:
- 'premises': the natural language premises
- 'premises-FOL': FOL formula annotation for the premises
- 'conclusion': the natural language conclusion
- 'conclusion-FOL': FOL formula annotation for the conclusion
- 'label': Truth value label for the conclusion
- 'story-id': story id (each story contains a set of premises and a set of conclusions)
- 'example-id': exampled id (each example contains a set of premises and one conclusion)
- 'source': whether the example is from the WikiLogic or HybLogic set. 

More details on the dataset, results and analyses can be found in our paper.

Code for evaluation with fine-tuning and few-shot prompting will be updated soon. 

## Citation
```
@article{han2022folio,
  title={FOLIO: Natural Language Reasoning with First-Order Logic},
  author = {Han, Simeng and Schoelkopf, Hailey and Zhao, Yilun and Qi, Zhenting and Riddell, Martin and Benson, Luke and Sun, Lucy and Zubova, Ekaterina and Qiao, Yujie and Burtell, Matthew and Peng, David and Fan, Jonathan and Liu, Yixin and Wong, Brian and Sailor, Malcolm and Ni, Ansong and Nan, Linyong and Kasai, Jungo and Yu, Tao and Zhang, Rui and Joty, Shafiq and Fabbri, Alexander R. and Kryscinski, Wojciech and Lin, Xi Victoria and Xiong, Caiming and Radev, Dragomir},
  journal={arXiv preprint arXiv:2209.00840},
  url = {https://arxiv.org/abs/2209.00840},
  year={2022}
```