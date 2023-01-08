# This repo is created for ML Reproducibility Challange 2022 
[for more information](https://paperswithcode.com/rc2022)
# Text2LIVE: Text-Driven Layered Image and Video Editing (ECCV 2022 - Oral)
## [<a href="https://text2live.github.io/" target="_blank">Project Page</a>]

>📋  A template README.md for code accompanying a Machine Learning paper

## Requirements

To install requirements:

```setup
pip install -r requirements.txt
```

## Training

#### Video Editing
Run the following command to start training
```
python train_video.py --example_config car-turn_winter.yaml
```
#### Image Editing
Run the following command to start training
```
python train_image.py --example_config golden_horse.yaml
```
Intermediate results will be saved to `results` during optimization. The frequency of saving intermediate results is indicated in the `log_images_freq` flag of the configuration.

## Results

### Reproduced Experiments

### Additional Experiments

## Acknowledgement

Link to Text2LIVE: [arxiv](https://arxiv.org/abs/2204.02491)
For more see the [supplementary material](https://text2live.github.io/sm/index.html).


## Citation
```
@article{bar2022text2live,
         title     = {Text2LIVE: Text-Driven Layered Image and Video Editing},
         author    = {Bar-Tal, Omer and Ofri-Amar, Dolev and Fridman, Rafail and Kasten, Yoni and Dekel, Tali},
         journal   = {arXiv preprint arXiv:2204.02491},
         year      = {2022}
}
```
