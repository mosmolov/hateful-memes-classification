# Hateful Memes Classification

If you would like to see the final project report with consolidated research and findings, navigate to the "FINAL_REPORT" document.

This repository contains code for classifying hateful memes using the Facebook Hateful Memes dataset.

## Libraries Used

This project uses the following core Python libraries:

* torch
* torchvision
* transformers
* scikit-learn
* matplotlib
* pandas
* numpy
* pillow

You can install the necessary libraries using pip:
```bash
pip install -r requirements.txt
```

## Recreating Results
The main workflow for data preparation, model training, and evaluation can be found in the Jupyter notebooks. To recreate the baseline results:

## Download the Dataset: 
The baseline/baseline_model.ipynb notebook includes steps to download the dataset using curl from Kaggle. You will need the Kaggle API set up or download it manually.

```bash
curl -L -o facebook-hateful-meme-dataset.zip "[https://www.kaggle.com/api/v1/datasets/download/parthplc/facebook-hateful-meme-dataset](https://www.kaggle.com/api/v1/datasets/download/parthplc/facebook-hateful-meme-dataset)"
unzip -q facebook-hateful-meme-dataset.zip -d hateful-memes
```
You can also download the dataset manually from Kaggle at [https://www.kaggle.com/datasets/parthplc/facebook-hateful-meme-dataset](https://www.kaggle.com/datasets/parthplc/facebook-hateful-meme-dataset) and place it in the hateful-memes directory.
## Unzip the Dataset:
Unzip the downloaded dataset to a directory named hateful-memes. The dataset contains three files:
* train.jsonl
* dev.jsonl
* test.jsonl
As well as the images in a subdirectory named img

## Install Dependencies:
Ensure all libraries listed in requirements.txt are installed using pip.
## Run the Baseline Notebook:
Execute the cells in baseline/baseline_model.ipynb sequentially

## Run the Experimentation Models:
The experimentation notebooks reflect the various models and techniques used to improve the baseline model. You can run these notebooks in a similar manner to the baseline notebook. They are named according to the different techniques used to improve the model
