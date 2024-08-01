# Solar Rooftop Detection from Publicly Available Satellite Imagery

## Acknowledgments
- The code used to train the model is adapted from Erfan Sobhaei's [Solar Panels Image Segmentation](https://www.kaggle.com/code/erfansobhaei/solar-panels-image-segmentation) notebook on Kaggle.

## Datasets Used
- [PV03](https://www.kaggle.com/datasets/salimhammadi07/solar-panel-detection-and-identification)
- [Rooftop Solar Panel Thailand](https://www.kaggle.com/datasets/johnsullivan66/rooftop-solar-panel-thailand)

## Instructions

### Model Training
- **`train_model_PV03.ipynb`**: This notebook is used to train the model on the PV03 dataset.

- **`train_model_T493.ipynb`**: This notebook is used to train the model on the Rooftop Solar Panel Thailand dataset, after it has been initially trained on the PV03 dataset. It can also be trained from scratch if **load_model** is set to `false`.

### Model Execution
- **`solar_panel_detection.ipynb`**: This notebook demonstrates how to utilize the trained model for solar panel detection.
- **`bkk1_02.tif`** in the **example-images** folder can be used to showcase the model. You will need to change the file paths yourself.

### Image and Mask Tiling
- **`ImageTiling/ImageTiling.ipynb`**: This notebook explains how shapefile masks are converted to raster masks and paired with their corresponding GeoTIFF files. Both the raster images and masks are then tiled to create the dataset for training the model.
- The example GeoTIFF file used in the notebook can be downloaded from [this link](https://drive.google.com/file/d/1jGJr4TNNiTTPQIOsirVG6sjBAH1vhqvW/view?usp=sharing).


### Image Enhancement
- **`ImageEnhancement/ImageEnhancement.ipynb`**: This notebook details the preprocessing image enhancement algorithms used on our datasets.