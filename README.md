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

<p align="center">
  <img src="images/cake.png" width="350" title="Cake">
  <img src="images/bread.png" width="350" title="Bread">
</p>

<p align="center">
  <img src="images/mountain.png" width="350" title="mountain">
  <img src="images/add-effect.png" width="350" title="add-effect">
</p>

Even though our GPU limitations, the model was found to be capable of the claims of the paper. Specifically, it was able to manipulate images in a semantically related and localized manner, without the need for handcrafted masks. The objective function was also able to effectively guide the localization of the generated edit. In addition, the model was able to successfully change textures and apply semi-transparent effects, as demonstrated by the outcomes of the experiments. Overall, these results support the effectiveness of the proposed method for text-driven and zero-shot image manipulat

### Additional Experiments

We investigated the asnwers of questions such as:

* What is the model's performance on applying material edits on non-smooth surfaces like fur?
* Does the color/texture similarity of the image and edit affects the performance of the edits?
* Does semantically related edits increase the performance? Or semantically meaningless edits drop the performance?
* Is the model able to perform reliable edits on complex structures like the human face? Does it preserve the facial structure of the human?

<p align="center">
  <img src="images/material.png" width="350" title="material">
  <img src="images/texture.png" width="350" title="texture">
</p>

<p align="center">
  <img src="images/emotions.png" width="350" title="emotions">
  <img src="images/beard.png" width="350" title="beard">
</p>


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
