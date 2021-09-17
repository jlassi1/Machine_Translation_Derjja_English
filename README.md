# Machine_Translation_Derjja_English
## Tunisian dialect(Derjja) to English Machine Translation with Google Seq2Seq and Transformer Model

This is an implementation of Machine Translation from Tunisian dialect(Derjja) to English using the Transformer Model and the sequence to sequence(seq2seq) Model which are state of the art pre-training models.

This repo is based on the code provided by the authors.

## Preprocessing

My data is composed of one column and each sentence or word has its translation below we split into 2 columns each has the Darija sentence and the other has the translation to English, then we concatenate them in one and save it.
Spliting Data to training and validation data.
converting our data to tensor using tf.data.Dataset.from_tensor_slices to be readable for the model 

| Black Wordcoud of Derjja word     | White Wordcoud of Derjja word     |
|------------|-------------|
| ![Splashscreen](https://github.com/jlassi1/Machine_Translation_Derjja_English/blob/main/asset/black_tunis.png)      | ![Splashscreen](https://github.com/jlassi1/Machine_Translation_Derjja_English/blob/main/asset/white_tunis.png)      |

more detail in [Data_Preprocessing.ipynb](https://github.com/jlassi1/Machine_Translation_Derjja_English/blob/main/models/Data_Preprocessing.ipynb)

## Training

For the Transformer, after a 150 epoch Loss: 0.0488, Accuracy: 0.3270

see the detail in [MT_with_Transfomer.ipynb](https://github.com/jlassi1/Machine_Translation_Derjja_English/blob/main/models/MT_with_Transfomer.ipynb)


For the Seq2Seq, after 100 epoch, batch_loss: 0.4867

see the detail in [MT_with_Seq2Seq.ipynb](https://github.com/jlassi1/Machine_Translation_Derjja_English/blob/main/models/MT_with_Seq2Seq.ipynb)

# Evaluation results

we still work on the bleu score ...

### Sample Translations
        the most accurate result from the Transformer model


Derjja (input)| English (output)
--- | --- |
مَهُوشْ رَاضِي عَلَى عِيشْتُو | unsatisfied with life.
عندي رنديفو غدوة الصباح | I have a meeting tomorrow.
فما فستفال فالحمامات غدوا | There is a festival in Hammamat tomorrow.

        the most accurate result from the Seq2Seq model

Derjja (input)| English (output)
--- | --- |
 شد إلكرسي من ساقو ورماه | he took the chair with his leg and threw it .
 خذينا الطيارة بش نمشيو لجربة | we took the flight to go to jerba .
 شد الحبل بالقوي وماتسيبوش | grab the rope well and dont let go .
 حسيتو شاد ڨارد وما يحبش حتى حد يقربلو والا يحكي معاه | i felt like he was on guard and didnt want anyone to come near him or talk with him .



## Dataset 

Dataset compart of 13036(sentences and words) rows 2 colmns('en', 'tn'), 12052 unique values in english and 12042 unique values in Derjja. Scraped from [DERJA NINJA](https://derja.ninja/)

![Splashscreen](https://github.com/jlassi1/Machine_Translation_Derjja_English/blob/main/asset/dataset_screenshot.png)

you can find the dataset used in this [Kaggle](https://www.kaggle.com/khawlajlassi/drejja-to-english) address. 

## AUTHORS
* Imen Ayari - [Githb](https://github.com/Immaannn2222)
             - [LinkedIn](https://www.linkedin.com/in/imene-ayari/  )
* Jacer Dabbabi - [Github](https://github.com/jaycer95)
             - [LinkedIn](https://www.linkedin.com/in/jacer-dabbabi-a1519a1a1/)
* Khawla Jlassi - [Github](https://github.com/jlassi1)
             - [LinkedIn](https://www.linkedin.com/in/khawla-jlassi/)

