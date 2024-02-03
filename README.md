# Movie Dialogue Chatbot using Sequence-to-Sequence with Attention  
This repository contains the implementation of a movie dialogue chatbot using sequence-to-sequence (Seq2Seq) architecture with attention mechanisms. The model is trained on the Cornell Movie Dialogues Corpus to generate responses in a conversation.  

## Dataset  
The model is trained on the Cornell Movie Dialogues Corpus, which contains a rich set of movie character dialogues. The dataset is preprocessed to create question-answer pairs for training.  

## Model Architecture  
The chatbot model consists of an Encoder-Decoder architecture with attention mechanisms. The key components include:  

Encoder: Utilizes a bidirectional Gated Recurrent Unit (GRU) to process input sequences and produce encoder hidden states.  

Attention Mechanism: Implements attention mechanisms (dot, general, concat) to focus on specific parts of the input sequence during decoding.  

Decoder: Employs a unidirectional GRU along with the attention mechanism to generate output sequences.  

## Training
The model is trained using teacher forcing, where the correct target outputs are used as inputs during training. Adam optimizer is employed for both the encoder and decoder.  

## Hyperparameters  
Hidden Size: 500  
Encoder and Decoder Layers: 2  
Dropout: 0.1  
Attention Model: Dot  
## Training Iterations  
The training process involves multiple iterations (epochs) over randomly sampled batches of dialogue pairs. The model parameters are saved at regular intervals.  

## Inference  
The trained model is capable of generating responses during inference using a Greedy Search Decoder. The chatbot takes user input and produces relevant responses based on the learned patterns from the movie dialogues.  


 
## Citation  
Jonathan P. Chang, Caleb Chiam, Liye Fu, Andrew Wang, Justine Zhang, Cristian Danescu-Niculescu-Mizil. 2020. "ConvoKit: A Toolkit for the Analysis of Conversations". Proceedings of SIGDIAL.

[ConvoKit](https://convokit.cornell.edu/)
