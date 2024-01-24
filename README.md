# Road Classification Using Satellite Images

This project focuses on the use of remote sensing technology and a UNet model with minimal parameters for efficient and accurate road network extraction from satellite images. The proposed approach has potential applications in traffic management, urban planning, disaster emergency response, and sustainable infrastructure development.

## Dataset
https://www.kaggle.com/datasets/balraj98/deepglobe-road-extraction-dataset
The dataset used in this project is available in the `data` folder, which contains four subfolders: `Train`, `Test`, `Valid`, and `Metadata`. The `Train` and `Test` folders contain images of roads and road masks, while `Metadata` contains satellite image paths of both test and train and also the mask path of the satellite images. The dataset includes 8570 images, including 6226 RGB satellite images with a resolution of 1024x1024 collected by the Digital Globe satellite.

## Training

To train the UNet model, run the `train.py` script. The script loads the dataset, preprocesses the images, and trains the model using the Adam optimizer and binary cross-entropy loss. The trained model is saved in the `models` folder.

## Testing

To test the trained model, run the `test.py` script. The script loads the test dataset, preprocesses the images, and evaluates the model on the test set. The results are saved in the `results` folder.

## Results

The proposed approach achieves high accuracy in road segmentation on publicly available datasets, including the Massachusetts Road Dataset, Deep Globe Road Extraction Challenge, and ISPRS 2D Semantic Labelling Contest.
