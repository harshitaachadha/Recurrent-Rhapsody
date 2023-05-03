# Recurrent-Rhapsody
The project titled “Recurrent Rhapsody: A Prompt-Driven Song Generation Pipeline” is an LSTM-based three-stage architecture that is designed to take in a text prompt and generate a music-lyrics combination that can be combined to create the next chart-topper *(well, not really)*. The project is aimed to produce an enhanced intelligence system by combining several machine learning models such as LSTM, Vanilla RNNs, and S-BERT.

The first part, an LSTM model generates lyrics of a song, given a prompt. This song is then fed into the second stage, a pre-trained hugging-face S-BERT model to generate a text embedding that is then matched to the existing database of embeddings using cosine similarity to obtain the MIDI track with the most similar lyrics to the one generated. This resultant track is then fed into an RNN model as the priming sequence to generate a new backing track. The lyrics along with this track are then output as the final results of the pipeline ready to be combined.

## Usage
To see the model in action, the Integration_Monster ipython notebook can be run to obtain real-time outputs! (Please bear in mind that to run this notebook, the public folder with stored models has to be present in the mounted g-drive - link to this has been provided in the notebook)

## Sample Output
![alt text](https://github.com/harshitaachadha/Recurrent-Rhapsody/blob/main/sample_op.png)
<iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/1505124808&color=%23ff5500&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true"></iframe><div style="font-size: 10px; color: #cccccc;line-break: anywhere;word-break: normal;overflow: hidden;white-space: nowrap;text-overflow: ellipsis; font-family: Interstate,Lucida Grande,Lucida Sans Unicode,Lucida Sans,Garuda,Verdana,Tahoma,sans-serif;font-weight: 100;"><a href="https://soundcloud.com/harshita-chadha-402075200" title="Harshita Chadha" target="_blank" style="color: #cccccc; text-decoration: none;">Harshita Chadha</a> · <a href="https://soundcloud.com/harshita-chadha-402075200/29apr-comp3-single" title="29apr Comp3 Single" target="_blank" style="color: #cccccc; text-decoration: none;">29apr Comp3 Single</a></div>

## License
[MIT](https://choosealicense.com/licenses/mit/)
