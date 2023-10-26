# Python Chatbot Project

This project aims to build a simple chatbot using neural networks and natural language processing techniques. The chatbot is trained on a dataset provided in the `intents.json` file, which contains patterns and responses.

## Table of Contents

- [Setup](#setup)
- [How It Works](#how-it-works)
- [Training](#training)
- [Usage](#usage)
- [License](#license)

## Setup

### Prerequisites

- Python 3.x
- Keras
- NLTK
- Numpy

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/elnaramammadova/my_chatbot.git
   ```

2. Navigate to the project directory and install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

## How It Works

The chatbot undergoes the following processes:

1. **Data Preprocessing**: The raw data is tokenized, and unnecessary characters are removed. The data is then lemmatized to reduce words to their base form.

2. **Training Data Creation**: Patterns are converted to a bag-of-words representation, and corresponding classes (intents) are encoded.

3. **Model Training**: The data is fed to a neural network, which learns to predict the intent of a given pattern.

## Training

The model architecture consists of:

- First layer: 128 neurons
- Second layer: 64 neurons
- Third layer: Neurons equivalent to the number of classes

The model is compiled with the Stochastic Gradient Descent (SGD) optimizer and trained for 200 epochs. The trained model is saved as `chatbot_model.h5`.

To train the model, run:

```bash
python train_chatbot.py
```

## Usage

After training, you can integrate the model with a user interface to get responses to user queries based on the trained intents.

```bash
python gui_chatbot.py
```

## License

This project is open-source. Feel free to use, modify, and distribute it as per your needs.
