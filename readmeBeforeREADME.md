# project structure
```text
Runners-On-XXXX
    |----papers
          |----2023.json
          |----2022.json
          |···
    |----src
          |----style.css
    |----script.py  
```

# Usage
1. Write `config.json` file including your repo name and the description of it.

2. The folder `papers` saves all papers you collected, and these papers classified by year(or other rule).

3. Run ```python script.py``` to generate README.md automatically.

4. Ignore the src/style.css, it doesn't work on github.

# Format of writing the information of a paper to json file
```json
[
  {
    "cite": "BibTeX Citation String copied here",
    "url": "paper link copied here",
    "code": "code address copied here"
  },
  {
    "cite": "@misc{su2021nonautoregressive,\n      title={Non-Autoregressive Text Generation with Pre-trained Language Models}, \n      author={Yixuan Su and Deng Cai and Yan Wang and David Vandyke and Simon Baker and Piji Li and Nigel Collier},\n      year={2021},\n      eprint={2102.08220},\n      archivePrefix={arXiv},\n      primaryClass={cs.CL}\n}",
    "url": "https://arxiv.org/abs/2102.08220",
    "code": "https://github.com/yxuansu/NAG-BERT"
  }
]
```

# Attention
If you clone this repo and then build your paper list repo, remember to delete .git/* and reinitialize it before pushing.
