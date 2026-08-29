This is a Jupyter Notebook for the pretraining of a Transformer decoder model from the ground-up using the TinyStories dataset (in particular, TinyStories-train.txt).
The dataset can be retrieved from: https://huggingface.co/datasets/roneneldan/TinyStories

The Jupyter notebook file is "decoder from scratch.ipynb", which contains the code to train the model and also inference.

The weights from my training are included as "minigpt_kv_model.pt", which you can load and run the model for inference without training.

The BPE tokeniser is stored in "tinystories_bpe_tokenizer.json", which has also been trained on the words in the TinyStories dataset.

The "train.bin" file contains the binarised id's of the tokens in the tokenizer. 
For example, token "cat" has id 60, then '60' is binarised as 00110110 00000000 00110000 00000000. (little endian)

---

You can think of this as an open-source model with open-weights.

---

Sample output:

<img width="2040" height="659" alt="1" src="https://github.com/user-attachments/assets/555fb75d-04ea-4bb5-9f4e-08f88b42daab" />

<img width="2087" height="331" alt="2" src="https://github.com/user-attachments/assets/c27f64d2-37bf-4990-aebb-1dfee77da908" />

