# Signformer
Official Code for the paper [Signformer is all you need: Towards Edge AI for Sign Language]

 
## Dataset and Feature Files Preparation
### Phoenix14T:
    wget "http://cihancamgoz.com/files/cvpr2020/phoenix14t.pami0.train"
    wget "http://cihancamgoz.com/files/cvpr2020/phoenix14t.pami0.dev"
    wget "http://cihancamgoz.com/files/cvpr2020/phoenix14t.pami0.test"


### Config updates
####Note that the default Feature Files directory is `./data`. If you download them to somewhere else, you need to update the `data` parameters in your config file:
    Phoenix14T:

    train: [PATH]/phoenix14t.pami0.train
    dev: [PATH]/phoenix14t.pami0.dev
    test: [PATH]/phoenix14t.pami0.test
    feature_size: 1024 (32x32)


* Install required packages using the `requirements.txt` file.
    `pip install -r requirements.txt`

* Remember after downloading sophiag, modify their __init__.py by removing the last:
`from sophia.sophia import SophiaG`


## Usage
### Train
  `python -m main train [CONFIG PATH]` 
### Test
  `python -m main test [CONFIG PATH] --ckpt [CHECKPOINT PATH]` 
