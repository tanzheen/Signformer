<h1 align="center"> Official: Signformer is all you need: Towards Edge AI for Sign Language
</h1>

[![arXiv](https://img.shields.io/badge/arXiv%20paper-2410.06940-b31b1b.svg)](https://arxiv.org/abs/2411.12901v1)&nbsp;
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/signformer-is-all-you-need-towards-edge-ai-1/gloss-free-sign-language-translation-on)](https://paperswithcode.com/sota/gloss-free-sign-language-translation-on?p=signformer-is-all-you-need-towards-edge-ai-1)



 
## Dataset and Feature Files Preparation
### Phoenix14T:
    wget "http://cihancamgoz.com/files/cvpr2020/phoenix14t.pami0.train"
    wget "http://cihancamgoz.com/files/cvpr2020/phoenix14t.pami0.dev"
    wget "http://cihancamgoz.com/files/cvpr2020/phoenix14t.pami0.test"

### Config
    train: [PATH]/phoenix14t.pami0.train
    dev: [PATH]/phoenix14t.pami0.dev
    test: [PATH]/phoenix14t.pami0.test

* Install required packages using the `requirements.txt` file.
    `pip install -r requirements.txt`

* Remember after downloading sophiag, modify their __init__.py by removing the last:
`from sophia.sophia import SophiaG`

## Usage
### Train
  `python -m main train [CONFIG PATH]` 
### Test
  `python -m main test [CONFIG PATH] --ckpt [CHECKPOINT PATH]` 

## BIBTEX
```bibtex
@misc{yang2024signformerneededgeai,
      title={Signformer is all you need: Towards Edge AI for Sign Language}, 
      author={Eta Yang},
      year={2024},
      eprint={2411.12901},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2411.12901}, 
}
```
