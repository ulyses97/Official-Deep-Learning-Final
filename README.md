# Official-Deep-Learning-Final
Final deep learning project where we compare and change parameters on YOLO segmentation models for pothole detection 
in order to run our code you will need to have jupyter notebook and download the raw jupyter notebook



## Dataset Setup 
The converted YOLO format dataset used in this project is avalialbe here in this link 
https://drive.google.com/file/d/1RHbNy7hZnzjcwUE8RkN2Rtk3ZTZnVoex/view?usp=sharing

When you finish downloading go into the `data.yaml` and change the pathing to where the files are located on your computer
`path: C:/Users/*change_to_your_path*/roadvis_yolo` change it to the correct path.

Here is the actual link of the dataset which is from roboflow and this would be downloaded as COCO segmentation format and then you would need to convert
into YOLO format which is already done with the google drive link but if you wanted to try and convert it here is the link. You would need to make an account on Roboflow to download the dataset:

https://universe.roboflow.com/sankritya-rai-cldft/roadvis-segmentation

If you decide to download the dataset on do the conversion on your own you do not need to worry about the pathing of the 
`data.yaml` it will have the correct path if you download it on your own. 

After downloading extract the zip file and rename the folder to `roadvis_yolo`

The folder should look like this:

```text
roadvis_yolo/
├── data.yaml
├── images/
│   ├── train/
│   ├── val/
│   └── test/
└── labels/
    ├── train/
    ├── val/
    └── test/
```
## Optinal:External Dataset Evaluation
A external dataset can be used if need be to test out the model on another dataset. The `roadvis_yolo` has a test folder
that already runs a test to see how well it performs on unseen data. This is just extra if you would like to use another dataset.


The external dataset that was used is **Pothole Detection v9i YOLOv8**.

Here is the link to the Roboflow website where the dataset is located at and this would be downloaded in YOLOv8 format and also you will need to create an account:

https://universe.roboflow.com/imacs-pothole-detection-wo8mu/pothole-detection-irkz9/dataset/9

This dataset was downloaded from Roboflow and has its own `train`, `valid`, and `test` folders along with a `data.yaml` file.

The notebook has the external dataset labeled as:

```python
external_dataset_name = "Pothole Detection v9i YOLOv8"
```

## Figures 
In the figures section are some of the plots that were given. Not all the plots are shown but rather it is 
the best results being tested. 

## Saved Results
In the saved results folder are the results that we were able to acheive from our testing. The files here are a summary of 
all the test we did and with the different parameters changed. Then the results of our best model being tested.

