# Brain Tumor Detection System using Convolutional Neural Networks (CNN)

## Project Overview

This project presents a robust system for the early and accurate detection of brain tumors from medical images (such as MRI or CT scans) using Convolutional Neural Networks (CNNs). Early and precise diagnosis of brain tumors is crucial for effective treatment planning and significantly improving patient prognosis. This system leverages advanced deep learning techniques combined with efficient image pre-processing to achieve high diagnostic accuracy.

The core of this system is a pre-trained Keras CNN model, specifically designed and trained to classify medical images, identifying patterns indicative of brain tumors.

## Features

* **Accurate Tumor Detection:** Utilizes a trained CNN model (`keras_model.h5`) for high-accuracy classification of brain images.
* **Automated Image Pre-processing:** Implements essential pre-processing steps (resizing, normalization) to prepare raw medical images for optimal model inference.
* **Web-based Interface:** (If you implement a Flask UI) Provides a user-friendly web interface via Flask for easy image uploads and instant diagnostic predictions.
* **Efficient Model Inference:** Optimized for quick prediction times, making it suitable for practical diagnostic support.
* **Reproducible Environment:** Managed dependencies via `requirements.txt` ensures easy setup and reproducibility.

## Technologies Used

* **Python:** The primary programming language.
* **TensorFlow / Keras:** For building, training (implied, as a pre-trained model is used), and loading the Convolutional Neural Network.
* **Flask:** (If you use it for the web interface) A lightweight web framework for the user interface.
* **Pillow (PIL):** For image manipulation and processing.
* **OpenCV (cv2):** Potentially used for advanced image processing tasks.
* **NumPy:** For numerical operations, especially array manipulation for image data.

## Project Structure
.
├── main.py                # Main Flask application (if applicable)
├── supportFile.py         # Contains core functions for image processing and model prediction
├── testCode.py            # Script for testing model prediction on individual images
├── keras_model.h5         # Pre-trained Convolutional Neural Network model
├── requirements.txt       # List of Python dependencies
├── info.csv               # (Optional) Data file, possibly for image information or dataset details
├── images/                # (Optional) Directory for sample images or dataset
│   └── example_image.png
└── README.md              # This file

*(Adjust the structure above if `main.py` is not a Flask app or if `images/` doesn't exist in your repo, or add other directories if present)*

## Setup and Installation

To set up and run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YourUsername/Brain-Tumor-Detection-CNN.git](https://github.com/YourUsername/Brain-Tumor-Detection-CNN.git)
    cd Brain-Tumor-Detection-CNN
    ```
    *(Replace `YourUsername` with your actual GitHub username)*

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    # On Windows:
    # venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Running the Web Application (if applicable)

If `main.py` is your Flask application:

1.  Ensure your virtual environment is active.
2.  Run the Flask application:
    ```bash
    python main.py
    ```
3.  Open your web browser and navigate to `http://127.0.0.1:5000/` (or the address displayed in your console).
4.  Upload a brain scan image to get the diagnosis.

### Running Test Predictions

To test the model on individual images using `testCode.py`:

1.  Ensure your virtual environment is active.
2.  (Optional) Place a test image in a designated folder or provide its path.
3.  Run the test script:
    ```bash
    python testCode.py
    ```
    *(You might need to modify `testCode.py` to point to a specific test image if it's not already set up to do so.)*

## Contributing

*(Optional: If you plan for others to contribute, add a section here)*
Feel free to fork this repository, open issues, or submit pull requests.

## License

*(Optional: You can add a license, e.g., MIT License)*
This project is open-sourced under the [MIT License](LICENSE).
