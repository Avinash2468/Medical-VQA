# Medical Visual Question Answering

## Abstract
This project focuses on medical visual question answering (VQA) using deep learning techniques. Specifically, we propose a simple but highly accurate VQA model that combines visual and language input encodings before passing them to a classifier. We conduct experiments using various vision and language encoders and demonstrate that the choice of encoder significantly impacts the model’s accuracy. Our results show that using novel vision encoders can achieve comparable accuracy to state-of-the-art models. Additionally, we provide a flexible and easy-to-use framework for training and testing VQA models with different encoders on medical VQA datasets. Overall, our work highlights the importance of encoder selection and offers a practical solution for VQA in the medical domain.

- For an indepth dive into the project, please refer to `report.pdf`.

## Setting up the environment
```
   conda env create -f environment.yml
``` 

## Changing the config
```
    # parameters that can be changed
    language_model_name : "emilyalsentzer/Bio_ClinicalBERT"
    vision_model_name : "convnext_base"
    experiment_name: "bioclinicalBERT_convnext"
```

## Training
``` 
    python train.py
```

## Testing
```
    python test.py
```
