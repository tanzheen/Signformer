# Official Code of Signformer is all you need
<p align="left">
<a href="" alt="arXiv">
    <img src="https://img.shields.io/badge/arXiv-2405.02730-b31b1b.svg?style=flat" /></a>
</p>


 
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
