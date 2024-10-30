# SMS Spam Detector

A machine learning application that classifies SMS messages as spam or not spam using a Linear Support Vector Classification (SVC) model. The application is deployed using Gradio to provide an interactive web interface for testing and predicting SMS messages.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)
- [Dependencies](#dependencies)
- [License](#license)

## Overview

The trained model uses Gradio, enabling users to input SMS messages and receive feedback if a text is classified as spam or not based on the model's performance.

## Features

- Data preprocessing and feature extraction using TF-IDF Vectorization.
- Classification using Linear Support Vector Classifier.
- Interactive web application interface using Gradio.
- Real-time prediction of SMS messages as spam or not spam.

## Dataset

The dataset used is the **SMSSpamCollection** dataset, which is a collection of 5,574 SMS messages tagged as either ham (legitimate) or spam. The dataset is included in the repository as `SMSSpamCollection.csv`.

## Installation

### Prerequisites

- Python 3.7 or higher
- pip package manager

### Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/ilikeitrhough/sms_spam_detector.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd sms_spam_detector
   ```

3. **Install the required dependencies:**

   ```bash
   pip install pandas scikit-learn gradio
   ```

## Usage

1. **Ensure the dataset file `SMSSpamCollection.csv` is in the project directory.**

2. **Run the application script:**

   ```bash
   python gradio_sms_text_classification.py
   ```

3. **Access the Gradio interface:**

   - After running the script, Gradio will provide a local URL (and optionally a public URL if `share=True` is set in the code).
   - Open the URL in your web browser to access the application.

4. **Predict SMS messages:**

   - Enter an SMS message into the input textbox.
   - Click the "Submit" button.
   - The application will display whether the message is spam or not.

## Testing

You can test the application using the following sample messages:

1. **You are a lucky winner of $5000!**
2. **You won 2 free tickets to the Super Bowl.**
3. **You won 2 free tickets to the Super Bowl. Text us to claim your prize.**
4. **Thanks for registering. Text 4343 to receive free updates on Medicare.**

## Dependencies

- **pandas**: For data manipulation and analysis.
- **scikit-learn**: For machine learning model building and evaluation.
- **Gradio**: For creating the interactive web interface.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.