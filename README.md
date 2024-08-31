# Solar Rooftop Detection from Publicly Available Satellite Imagery

## Acknowledgments
- The code used to train the model is adapted from Erfan Sobhaei's [Solar Panels Image Segmentation](https://www.kaggle.com/code/erfansobhaei/solar-panels-image-segmentation) notebook on Kaggle.

## Dataset Used
- [VatSaiKhlongSaphanSung+V280](https://www.kaggle.com/datasets/johnsullivan66/vatsaikhlongsaphansung/data)

## Advisements
- **TensorFlow Versioning**: The notebooks were developed using TensorFlow 2.15 and Keras 2.15. Please note that models saved with versions earlier than TensorFlow 2.16 may not be compatible with version 2.16. If you encounter any issues related to TensorFlow, consider downgrading to an earlier version.

## Instructions

### Model Training
- **`train_and_evaluate_model.ipynb`**: This notebook is used to train and evaluate the model on the VatSaiKhlongSaphanSung+V280 dataset.

### Model Execution
- **`solar_panel_detection.ipynb`**: This notebook demonstrates how to utilize the trained model for solar panel detection.
- **`village_test1.tif`** in the **example-images** folder can be used to showcase the model. You will need to change the file paths yourself.

### Image and Mask Tiling
- **`ImageTiling/ImageTiling.ipynb`**: This notebook explains how shapefile masks are converted to raster masks and paired with their corresponding GeoTIFF files. Both the raster images and masks are then tiled to create the dataset for training the model.
- The example GeoTIFF file used in the notebook can be downloaded from [this link](https://drive.google.com/file/d/1jGJr4TNNiTTPQIOsirVG6sjBAH1vhqvW/view?usp=sharing). Place this image in the **`ImageTiling/image_geotiff`** folder.