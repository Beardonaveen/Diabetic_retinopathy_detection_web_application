# Diabetic_retinopathy_detection_web_application
This project uses TensorFlow and Flask to create a web application that classifies images as 'Infected' or 'Uninfected'. Users upload an image, and the model, trained on labeled data, processes the image to predict its category. The app then displays the prediction along with the accuracy, providing a simple interface for real-time images
Here's a sample README file for your project:

---

# Diabetic Retinopathy Detection

This project is a web-based application designed to classify images as 'Infected' or 'Uninfected' using a deep learning model built with TensorFlow and Keras. The application is powered by Flask and allows users to upload images, which are then processed by the model to predict the category of the image.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Model Details](#model-details)
- [Contributing](#contributing)
- [License](#license)

## Overview

This application utilizes a Convolutional Neural Network (CNN) to classify images into two categories: 'Infected' and 'Uninfected'. The model is trained on a labeled dataset and deployed using Flask to create a user-friendly web interface. Users can upload an image, and the application will return the predicted label and the accuracy of the prediction.

## Features

- **Real-Time Image Classification:** Upload images and get instant predictions.
- **User-Friendly Interface:** Simple and intuitive design using HTML and Bootstrap.
- **Accuracy Display:** View the model's confidence level in its predictions.

## Project Structure

```
├── diabetic-retinopathy-detection-main/
│   ├── Deploy/
│   │   ├── model.h5            # Pre-trained model file
│   │   ├── app.py              # Flask application
│   │   ├── static/
│   │   │   ├── background.jpeg # Background image for the UI
│   │   ├── templates/
│   │   │   ├── index.html      # Home page
│   │   │   ├── home.html       # Other HTML files
│   │   │   ├── predict.html    # Prediction results page
│   ├── uploads/                # Directory where uploaded images are stored
```

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/your-username/diabetic-retinopathy-detection.git
   cd diabetic-retinopathy-detection-main/Deploy
   ```

2. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Download the Model:**
   Ensure you have the `model.h5` file in the `Deploy` directory. If not, place your pre-trained model in this directory.

4. **Run the Application:**

   ```bash
   python app.py
   ```

5. **Access the Application:**
   Open your web browser and go to `http://127.0.0.1:5001/`.

## Usage

- **Home Page:** Navigate to the home page and upload an image file.
- **Prediction:** Once uploaded, the application will display the predicted category ('Infected' or 'Uninfected') and the model's accuracy.

## Model Details

- **Model Architecture:** The model is a Convolutional Neural Network (CNN) designed to process images of size 64x64 with 3 color channels (RGB). It outputs predictions for two categories: 'Infected' and 'Uninfected'.
- **Input Size:** `(64, 64, 3)`
- **Output Classes:** 
  - `0: Infected`
  - `1: Uninfected`

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This README provides an overview of the project, instructions for installation and usage, as well as details about the model and the application's features.
