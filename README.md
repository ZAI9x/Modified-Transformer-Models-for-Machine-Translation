# Modified Transformer Models for Machine Translation (Portuguese to English)

## Introduction
In our project, we developed a modified Transformer model for Portuguese to English machine translation. Our modifications included adding a Masked Multi-Head Attention component to the encoder, and also experimenting with different feedforward architectures such as ResNet, CNN, and LSTM. We also removed the encoder and decoder parts of the Transformer model interchangeably to evaluate their importance in the architecture. Through careful evaluation and comparison with the original performance, we gained insights into the strengths and weaknesses of different architectural choices for machine translation tasks. Our project highlights the flexibility and adaptability of the Transformer model architecture, and demonstrates the importance of experimentation in improving translation quality and training efficiency.

## Features of the project
Features of Actual Transformer-Model are:
+ Self-Attention Mechanism: The Transformer relies heavily on self-attention mechanisms, which allow each word in the input sequence to attend to other words, capturing dependencies and relationships across the entire sequence. Self-attention enables the model to consider context from different positions without explicitly using recurrent or convolutional layers.
  
+ Multi-Head Attention: The Transformer employs multiple attention heads to capture different types of information. Each head performs a separate weighted sum over the input sequence, providing multiple perspectives and enhancing the model's ability to attend to different parts of the sequence simultaneously.
  
+ Positional Encoding: Since Transformers do not have recurrent or convolutional operations that inherently capture sequence order, positional encoding is introduced to incorporate positional information. Positional encodings are added to the input embeddings and provide the model with a sense of word order.
  
+ Encoder-Decoder Structure: The Transformer architecture consists of an encoder and a decoder. The encoder processes the input sequence and produces a representation that captures the input's contextual information. The decoder takes this representation and generates the output sequence step by step.
  
+ Residual Connections and Layer Normalization: Residual connections are used throughout the Transformer architecture to mitigate the vanishing gradient problem and improve gradient flow during training. Layer normalization is applied after each sub-layer to stabilize the learning process and improve the model's ability to generalize.
  
+ Feedforward Neural Networks: The Transformer incorporates feedforward neural networks with position-wise fully connected layers. This allows each position in the sequence to be processed independently and nonlinear transformations to be applied to capture complex patterns and features.
  
+ Masking: Masking is applied to the decoder's self-attention layer to prevent it from attending to future positions during training, ensuring that each prediction only depends on previously generated outputs.

## Modifications of the project
+ Modifying the Feedforward Part
o CNN layers, residual connections, and layer normalization , Relu activation
o Convolutional Layer: GELU (Gaussian Error Linear Unit) Activation
o LSTM , Relu Activation
o Resnet 2 layers with skip connections.
+ Modified the Encoder and Decoder inner Architecture.
+ Removing the Encoder Part
+ Removing the Decoder Part


## Sources:
+	https://colab.research.google.com/drive/1OMCcIEhH3qTGPy_1Z59akDFm9m9HeTPv
+ https://www.kaggle.com/datasets/samirmoustafa/arabic-to-english-translation-sentences
+ https://proceedings.neurips.cc/paper_files/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aaPaper.pdf
+ https://colab.research.google.com/drive/1NhHSfbeIGHQmNr36Y4ytpGKLLdUy0MYm#scrollTo=lDzIyhhpEMgp
