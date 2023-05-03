# Recurrent-Rhapsody
The project titled “Recurrent Rhapsody: A Prompt-Driven Song Generation Pipeline” is an LSTM-based three-stage architecture that is designed to take in a text prompt and generate a music-lyrics combination that can be combined to create the next chart-topper *(well, not really)*. The project is aimed to produce an enhanced intelligence system by combining several machine learning models such as LSTM, Vanilla RNNs, and S-BERT.

The first part, an LSTM model generates lyrics of a song, given a prompt. This song is then fed into the second stage, a pre-trained hugging-face S-BERT model to generate a text embedding that is then matched to the existing database of embeddings using cosine similarity to obtain the MIDI track with the most similar lyrics to the one generated. This resultant track is then fed into an RNN model as the priming sequence to generate a new backing track. The lyrics along with this track are then output as the final results of the pipeline ready to be combined.

## Usage
To see the model in action, the Integration_Monster ipython notebook can be run to obtain real-time outputs! (Please bear in mind that to run this notebook, the public folder with stored models has to be present in the mounted g-drive - link to this has been provided in the notebook)

## Sample Output
![alt text](https://github.com/harshitaachadha/Recurrent-Rhapsody/blob/main/sample_op.png)
[Listen to the backing track on SoundCloud](https://soundcloud.com/harshita-chadha-402075200/29apr-comp3-single?si=08c59c193b9c44858b2b3cb3a1137abe&utm_source=clipboard&utm_medium=text&utm_campaign=social_sharing)

## License
[MIT](https://choosealicense.com/licenses/mit/)
