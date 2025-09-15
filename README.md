# 🐐 Livestock Health Monitoring with Deep Learning

## Project Overview

This project implements a deep learning solution for monitoring the health of livestock, specifically goats, using image classification. The goal is to automatically classify goats as either **Healthy** or **Unhealthy** based on visual data, providing an early warning system for farmers and veterinarians.

## Features

*   **Image-based Classification:** Utilizes Convolutional Neural Networks (CNNs) to analyze images of goats.
*   **Health Status Prediction:** Predicts whether a goat is healthy or unhealthy.
*   **PyTorch Implementation:** Built using the PyTorch deep learning framework.
*   **Data Preprocessing:** Includes image resizing, augmentation (random horizontal flip, rotation), and normalization.
*   **Model Training & Evaluation:** Comprehensive training loop with validation and testing to ensure model performance.

## How it Works

The core of this project is a custom-built CNN model designed to learn features from goat images. The model is trained on a dataset of labeled images (healthy/unhealthy goats). During inference, it takes a new goat image as input and outputs a prediction of its health status.

## Technologies Used

*   **Python**
*   **PyTorch**: Deep Learning Framework
*   **torchvision**: For dataset loading and image transformations
*   **scikit-learn**: For data splitting and evaluation metrics
*   **NumPy**: For numerical operations
*   **PIL (Pillow)**: For image processing

## Getting Started

### Prerequisites

To run this project, you will need:

*   Python 3.x
*   pip (Python package installer)
*   A dataset of goat images, organized into `healthy_goat` and `unhealthy_goat` subdirectories (e.g., `D:\goats\healthy_goat`, `D:\goats\unhealthy_goat`).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Narcisse1/LivestockHealthMonitoring.git
    cd LivestockHealthMonitoring
    ```

2.  **Install dependencies:**
    ```bash
    pip install torch torchvision scikit-learn numpy Pillow
    ```

### Training the Model

1.  **Prepare your dataset:** Place your goat images in a directory structure like this:
    ```
    your_dataset_path/
    ├── healthy_goat/
    │   ├── image1.jpg
    │   ├── image2.png
    │   └── ...
    └── unhealthy_goat/
        ├── imageA.jpg
        ├── imageB.png
        └── ...
    ```

2.  **Update `goatHealth.ipynb`:** Open `goatHealth.ipynb` (or convert it to a Python script) and modify the `DATASET_PATH` variable to point to your dataset directory:
    ```python
    DATASET_PATH = "/path/to/your/goat_dataset" # e.g., "C:\\Users\\YourUser\\Documents\\goats"
    ```

3.  **Run the notebook/script:** Execute the cells in `goatHealth.ipynb` to train the model. The trained model will be saved as `goat_classifier.pth`.

## Model Architecture

The project uses a custom Convolutional Neural Network (`GoatCNN`) with the following layers:

*   Three convolutional layers with ReLU activation and max-pooling.
*   A fully connected layer.
*   A dropout layer for regularization.
*   An output layer for binary classification.

## Results

The `goatHealth.ipynb` notebook provides evaluation metrics such as accuracy, classification report, and confusion matrix on the test set, demonstrating the model's performance in distinguishing between healthy and unhealthy goats.

## Contributing

Contributions are welcome! Please feel free to fork the repository, make improvements, and submit pull requests.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Author
# Narcisse Ndongkain
# ndongkainnarcisse@gmail
---

![Smart Goat Farming in Kenya](https://private-us-east-1.manuscdn.com/sessionFile/B0YB49ZDHs7DmiBg985JtQ/sandbox/zYjG2w78LpxsP5c0X7V875-images_1757945466478_na1fn_L2hvbWUvdWJ1bnR1L0xpdmVzdG9ja0hlYWx0aE1vbml0b3Jpbmcvc21hcnRfZ29hdF9mYXJtaW5n.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvQjBZQjQ5WkRIczdEbWlCZzk4NUp0US9zYW5kYm94L3pZakcydzc4THB4c1A1YzBYN1Y4NzUtaW1hZ2VzXzE3NTc5NDU0NjY0NzhfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwweHBkbVZ6ZEc5amEwaGxZV3gwYUUxdmJtbDBiM0pwYm1jdmMyMWhjblJmWjI5aGRGOW1ZWEp0YVc1bi5qcGciLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3OTg3NjE2MDB9fX1dfQ__&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=ENZaOyutGOANg~7iZe2afeyRnjtoCpEGGNrNtlU~mUpOXv8XqSXbUHRiE2v4BF~6mIsX5k8okGQ-me8ilYCBjddpDxMXkzZawFE6t92kdG9BIeniuMkdEGZ8ZmoDrZdh4e~6ooBg5HIl10fEKU0IGi930Fey3x8xAbOxYEda1r5mHvpcQT8D7zPz1FJuPPXqwUXui3uUyDo5JoEfJEQrsGHPILcFC4KslYBstSCFktCi4APK5Pp5-6cmVwQBf4IEqMI353hxTrKTtzi-380kxrf3P-IWDM6MJwGy2R3H9DYTcYlYygnJkk~jfHcpeY~8CuyDySQlZRoasXdSkPiFfg__)

*Image Source: AI & IoT in Goat Farming: How Smart Tech is Revolutionizing Herd Health Monitoring*
