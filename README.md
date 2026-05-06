# Official-Deep-Learning-Final
Final deep learning project where we compare and change parameters on YOLO segmentation models for pothole detection 



## Dataset Setup 
The converted YOLO format dataset used in this project is avalialbe here in this link 
https://drive.google.com/file/d/1lV8izgPy237dOdAs0H5UhNDijqjbYx0c/view?usp=sharing

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

## External Dataset Evaluation
A external dataset was used to test how well the model would perfom to new data

The external dataset that was used is **Pothole Detection v9i YOLOv8**.

Here is the link to the Roboflow website where the dataset is located at:
https://universe.roboflow.com/imacs-pothole-detection-wo8mu/pothole-detection-irkz9/dataset/9

This dataset was downloaded from Roboflow and has its own `train`, `valid`, and `test` folders along with a `data.yaml` file.

The notebook has the external dataset labeled as:

```python
external_dataset_name = "Pothole Detection v9i YOLOv8"
