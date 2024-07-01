# SMS Spam Detection Using Python

## Overview
This project focuses on developing a machine-learning model to detect spam SMS messages. By training the model on a dataset with labeled examples of both spam and non-spam (ham) messages, we aim to create a reliable and accurate classifier to identify and filter spam messages.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Results](#results)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Installation
To set up and use this project, follow these steps:

1. Clone the repository:
   ```bash
   # Clone the repository to your local machine
   git clone https://github.com/ArmanThakur-1001/SMS_SPAM_DETECTION.git
   cd SMS_SPAM_DETECTION
   ```

2. Install the required dependencies:
   ```bash
   # Install the required Python packages
   pip install -r requirements.txt
   ```

## Usage
After installing the dependencies, you can use the trained model to predict whether a given SMS message is spam or ham. Here's an example:

```python
# Import the SpamDetector class
from sms_spam_detection import SpamDetector

# Load the trained model
model = SpamDetector.load_model("path/to/your/model")

# Define an SMS message for prediction
message = "Congratulations! You've won a free cruise."

# Predict whether the message is spam or ham
result = model.predict(message)

# Print the prediction result
print(f"Prediction: {result['class']} (Probability: {result['probability']})")
```

## Dataset
The dataset used for training and evaluation is located in directory. It includes labeled examples of spam and ham messages. You can replace it with your dataset if needed.

## Model Training
Train the Model.

## Evaluation
The model's performance is evaluated on a separate test set. Evaluation metrics such as accuracy, precision, recall, and F1 score are calculated.

## Results
A summary of the model's performance are shown. 

## Dependencies
This project requires:
- Python 3.x
- scikit-learn
- pandas
- numpy
- matplotlib
