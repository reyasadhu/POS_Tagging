# Part-of-Speech Tagging using Hidden Markov Model

This project implements a Part-of-Speech (POS) tagging system using a Hidden Markov Model (HMM). The model is trained on the `conll2000` dataset from the NLTK library.

## Requirements

- Python 3.x
- numpy
- pandas
- scikit-learn
- nltk

## Installation
 ```bash
    pip install numpy pandas scikit-learn nltk
 ```
## Hidden Markov Model (HMM)

A Hidden Markov Model (HMM) is a statistical model that represents a system which transitions between hidden states. It is particularly useful for tasks where the system being modeled is assumed to be a Markov process with unobserved (hidden) states.

### Key Components of HMM:
1. **States**: The hidden states of the model.
2. **Observations**: The observed events that are dependent on the hidden states.
3. **Transition Probabilities**: The probabilities of transitioning from one state to another.
4. **Emission Probabilities**: The probabilities of observing a particular observation from a state.
5. **Initial State Probabilities**: The probabilities of the system starting in each state.

### Applications of HMM:
- Part-of-speech tagging
- Speech recognition
- Bioinformatics (e.g., gene prediction)
- Time series analysis

In this notebook, we use HMM for part-of-speech tagging, where:
- States represent the part-of-speech tags.
- Observations represent the words in the sentences.
- Transition probabilities represent the likelihood of a tag following another tag.
- Emission probabilities represent the likelihood of a word being associated with a tag.
- Initial state probabilities represent the likelihood of a tag being the start of a sentence.

## Viterbi Algorithm:
The Viterbi algorithm is a dynamic programming algorithm used for finding the most likely sequence of hidden states (tags) given a sequence of observed events (words).

For more details on the Viterbi algorithm in part-of-speech tagging, you can refer to this [link]([https://medium.com/analytics-vidhya/parts-of-speech-pos-and-viterbi-algorithm-3a5d54dfb346]).
