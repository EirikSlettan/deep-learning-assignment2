# Grapheme-to-Phoneme Conversion using Seq2Seq LSTMs

Assignment for the course CSC3042F AI: Deep Learning at the University of Cape Town (UCT)

This project implements a grapheme-to-phoneme (G2P) model using sequence-to-sequence LSTM architectures in PyTorch.

The goal is to convert written words into phoneme sequences and compare different decoder context mechanisms.

## Models Implemented

- Seq2Seq without context
- Seq2Seq with fixed context vector
- Seq2Seq with attention

The models use a custom LSTM cell implemented from scratch rather than PyTorch’s built-in `nn.LSTM`.

## Dataset

The dataset consists of:

- Input word
- Corresponding phoneme sequence

Example:

| Word | Phonemes |
| ---- | -------- |
| cat  | K AE T   |

Special tokens used:

```text
<PAD> <SOS> <EOS> <UNK>
```
