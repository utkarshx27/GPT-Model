# Language Model for Shakespearean Text Generation using Transformers

## Description
This project focuses on creating a language model capable of generating new text in the style of William Shakespeare's poems. The model is based on the Transformer architecture, a powerful deep learning model known for its ability to handle sequential data effectively. With this project, we aim to showcase the capabilities of the Transformer architecture in natural language processing tasks.

## Dataset

The training data consists of a compilation of all the poems of William Shakespeare. The dataset is provided as a plain text file containing the poems' text. We preprocess the data to extract unique characters as the vocabulary and convert the text into numerical form for feeding into the model.

## Implementation

The implementation of the project involves building a Bigram Language Model using PyTorch. The model includes custom implementations of multi-head self-attention and feedforward layers, which form the core components of the Transformer architecture. The model learns to predict the next character in a sequence given the previous context, effectively mimicking the writing style of Shakespeare.

## Training and Optimization

To train the model, we use the AdamW optimizer and minimize the cross-entropy loss between the predicted characters and the actual characters in the training data. The training process continues for a predefined number of iterations, and the model's performance is evaluated periodically on both the training and validation sets.

## Generating New Text

After training the language model, we can use it to generate new text in Shakespearean style. Starting with a seed text, the model predicts the next character and appends it to the seed, forming a new context for the next prediction. This process is repeated iteratively to generate longer passages of text.

## Results and Evaluation

The project's performance is evaluated based on the fluency and coherence of the generated text. While the model may not perfectly replicate Shakespeare's writing style, we expect it to capture some of the essential characteristics, such as archaic language, poetic phrasing, and use of metaphors.

## Dependencies

To run this project, you need the following dependencies:

- PyTorch
- TorchVision
- NumPy
## Usage

Clone the repository: git clone https://github.com/utkarshx27/transformer-shakespeare.git
Install the required dependencies: pip install torch torchvision numpy
Train the language model: python train.py
Generate new text: python generate.py
## Contributing

We welcome contributions to improve the model's performance, add new features, or enhance the codebase. Please fork the repository, create a new branch for your changes, and submit a pull request.
