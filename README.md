
# COVID-19 Detection and Localization on Chest Radiographs

This project detects and localizes COVID-19 abnormalities in chest radiographs using computer vision techniques. COVID-19 has presented significant diagnostic challenges as its pulmonary appearance often resembles other types of pneumonia. This model aims to assist radiologists and non-radiologists in making quick, confident diagnoses by detecting and localizing disease patterns in radiographic images.

## Table of Contents
- [COVID-19 Detection and Localization on Chest Radiographs](#covid-19-detection-and-localization-on-chest-radiographs)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Dependencies](#dependencies)
  - [Task Description](#task-description)
  - [Usage](#usage)
  - [License](#license)

## Installation

To set up the environment, ensure you have Python installed, and then install the necessary packages:

```bash
# Install required packages
pip install pandas numpy pillow tqdm pydicom python-gdcm ultralytics pylibjpeg-libjpeg opencv-python
```

## Dependencies

This project requires the following libraries:

- **Pandas**: Data manipulation and processing
- **NumPy**: Numerical operations and array handling
- **Pillow (PIL)**: Image processing
- **TQDM**: Progress bars for dataset processing
- **PyDicom**: Handling of DICOM images, a standard in medical imaging
- **Python-GDCM**: Support for compressed DICOM files
- **Ultralytics**: Model handling and computer vision tasks
- **Pylibjpeg**: Efficient JPEG encoding/decoding for DICOM images
- **OpenCV**: Image processing for bounding box visualizations

Ensure all dependencies are installed before running the notebook.

> **Note**: To use project weights, please download best.pt from [here](https://drive.google.com/drive/folders/1eEHI0Gr1bc7exR8aIlAL8R4vIaAE0eh9?usp=drive_link)

## Task Description

The goal of this notebook is to detect and localize COVID-19 abnormalities in chest radiographs. Specifically, the notebook covers:

- **Data Loading**: Converting DICOM images into JPEG format for easier processing.
- **Model Training**: Training a model to classify and localize COVID-19 patterns, including bounding box annotation.
- **Evaluation**: Assessing the model’s performance using metrics suitable for localization and classification.

This project uses data and annotations provided by radiologists in collaboration with the Society for Imaging Informatics in Medicine (SIIM), FISABIO, BIMCV, and RSNA.

## Usage

1. Clone this repository and navigate to the directory.
2. Run the notebook in a Jupyter environment:

   ```bash
   jupyter notebook covid19-detection.ipynb
   ```

3. Follow the notebook cells sequentially to process images, train the model, and evaluate its performance.

> **Note**: This project aims to assist medical professionals by localizing potential COVID-19 patterns in chest radiographs and should not be used as a sole diagnostic tool.

## License

This project is open-source and available under the MIT License.
