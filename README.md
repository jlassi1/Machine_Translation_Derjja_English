# Machine_Translation_Derjja_English
## Tunisian dialect(Derjja) to English Machine Translation with Google Seq2Seq and Transformer Model

This is an implementation of Machine Translation from Tunisian dialect(Derjja) to English using the Transformer Model and the sequence to sequence(seq2seq) Model which are state of the art pre-training models.

This repo is based on the code provided by the authors.

## Preprocessing

My data is composed of one column and each sentence or word has its translation below we split into 2 columns each has the Darija sentence and the other has the translation to English, then we concatenate them in one and save it.
Spliting Data to training and validation data.
converting our data to tensor using tf.data.Dataset.from_tensor_slices to be readable for the model 

|------------|-------------|
| ![Splashscreen](https://github.com/jlassi1/Machine_Translation_Derjja_English/blob/main/asset/black_tunis.png) | ![Splashscreen](https://github.com/jlassi1/Machine_Translation_Derjja_English/blob/main/asset/white_tunis.png)  

## Training

# Evaluation results



### Sample Translations
Derjja (in)| English (out)
--- | --- |
مَهُوشْ رَاضِي عَلَى عِيشْتُو | unsatisfied with life.
عندي رنديفو غدوة الصباح | I have a meeting tomorrow.
فما فستفال فالحمامات غدوا | There is a festival in Hammamat tomorrow.




## AUTHORS
* Imen Ayari - [Githb](https://github.com/Immaannn2222)
             - [LinkedIn](https://www.linkedin.com/in/imen-ayari1-77312a1a2/)
* Jacer Dabbabi - [Github](https://github.com/jaycer95)
             - [LinkedIn](https://www.linkedin.com/in/jacer-dabbabi-a1519a1a1/)
* Khawla Jlassi - [Github](https://github.com/jlassi1)
             - [LinkedIn](https://www.linkedin.com/in/khawla-jlassi-11941019a/)

