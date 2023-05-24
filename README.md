# Dialogue Classification using **Bidirectional Encoder Representations from Transformers** (BERT)
A dialogue classifier from the show The Office. This code utilises the fine-tuned BERT-based model to classify the dialogues as Jim or Dwight's Dialogues.

# Jim vs. Dwight Dialogue Speaker Classification

This project focuses on classifying speakers in TV series dialogues using a fine-tuned BERT-based model. The model is trained on a dataset containing dialogues from the TV series "The Office" and can predict the speaker of the line with a 84% accuracy.

## Dataset

The dataset used in this project consists of dialogues from The Office.
Note: The model was only trained on the dialogues given in the file `train.csv` for a Kaggle competition by IEEE NITK's Computer Intelligence Society.

## Requirements

- TensorFlow
- Transformers
- Pandas
- NumPy

## Application

1. About the dataset:
   - The training dataset was in CSV format with columns: "id", "line", "speaker".
   - The validation dataset was split from the `train.csv` file, hence it is also in the the same format.
   - Data was properly cleaned and pre-processed.

2. Fine tuning the BERT model:
   - Run the `BERT-ieeekagglecup-2023.ipynb` notebook to fine-tune the BERT model on the training dataset.
   - The notebook tokenizes the text, prepares input tensors, and trains the model.

3. Evaluation:
   - The trained model is evaluated on the validation dataset using accuracy and classification report metrics.
   - The evaluation results can be used to assess the model's performance.

4. Making predictions:
   - Use the trained model to predict the speaker of dialogue lines.
   - `test.csv` dataset is in CSV format with columns: "id", "line".

5. Generated the submission CSV for the Kaggle Contest - my first one :)

Feel free to contribute, open issues, or submit pull requests to enhance the project!

