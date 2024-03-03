# Music-Genre-Classification
We have always been told by music companies about the genre of a music that this song is of this genre and that song of another genre. But most of us are unaware of how the genre of a song is decided. 
Well, this repository is made to addrss this issue. 
The repository focuses on deriving various features of a song such as MFCCS, Chromagram, RMS, etc. to classify between six different genres such as Pop, Funk, etc.

Explanation of what each file compries of:
1. Making Data.ipynb
The songs were downloaded from the internet and were imported in the jupyter notebook by the help of 'Librosa' library of Python3 and the waveform of the audio file was plotted. Next, features such as MFCCS, Chromagram, RMS, Zero Crossings and Tempo of each song was extracted and saved in a CSV file.

2. Preprocessing.ipynb
Preprocessing of a raw data is very crucial in any project. The features were checked for any null values or outliers, particularly MFCCS and Zero crossings were scaled and the refined data was then saved in a CSV file.

3. MFCCS Preprocessing.ipynb
The aim is to use every feature one by one to predict the genre of a song and use the majority prediction to quote the final genre. Here is an example of how ANN is used to predict the genre. In this file, the raw MFCCS data is preprocessed and ANN model is used for prediction. The accuracy is whopping 0.9275 on the test dataset and 0.9268 on the train dataset.

4. Countour.ipynb
The spectogram with contour lines of the song is plotted for better understanding. The 'audio waveform', 'Mel spectogram' and 'chromagram' has also been plotted. Lastly a 3-D spectogram with x, y, and z axes as Time, frequency, and amplitude is been plotted. 
