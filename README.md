# Shoe_Pair_Data_Exploration
This repository contains a Jupyter notebook that performs data loading, preprocessing, and visualization for a computer vision task. The notebook is specifically designed to work with a dataset of shoe images, identifying and creating pairs of "same" and "different" image pairs.
The output includes a visual comparison of these pairs to prepare the data for further machine learning model training.

This notebook was developed in Google Colab, and you will need to connect a Google Drive to access the dataset.

Prerequisites

    Google Colab environment

    A Google Drive connected to your Colab environment

    A dataset of shoe images in the specified folder format: /content/gdrive/My Drive/data-ex2/data/train/. The notebook expects image filenames to include _left_ or _right_ to identify the shoe type, and a common identifier to link pairs.

Dependencies

The following Python libraries are required to run the notebook:

    pandas and numpy: For data manipulation and numerical operations.

    matplotlib: For data visualization and plotting.

    torch, torch.nn, and torch.optim: The core PyTorch libraries for building neural networks.

    Pillow (PIL): For loading and manipulating image files.

    glob and os: For file system operations.

Execution

    Upload the vision_ex2.ipynb file to your Google Colab environment.

    Run the first code cell to import the necessary libraries.

    Run the second code cell to mount your Google Drive.

    Ensure your dataset is correctly placed in the specified folder structure on your Google Drive (/content/gdrive/My Drive/data-ex2/data/train/).

    Run the remaining cells sequentially to process the data and generate the visualizations.

Code Overview

The notebook performs the following key steps:

    Data Pairing: The script iterates through the dataset folder to identify and pair left and right shoe images.

    Data Validation: It counts the total number of valid pairs found to ensure the dataset is correctly processed.

    Image Loading and Resizing: A utility function is defined to load images, convert them to RGB, and resize them to a standard 224x224 pixel size.

    Pair Generation: Separate functions are used to create "same pairs" and "different pairs" for comparative visualization and potential model training.

    Visualization: The notebook concludes by plotting a single "same pair" and a single "different pair" to visually demonstrate the output.
