# Extract-Information-using-Rule-Based-Methods
Information extraction Interview Task</br>

## Folders
Score/Summary in csv folder </br>
xml of pdf of research paper in xml folder</br>
pdf of researchpaper in papaer folder 

## Task
1. Use TFIDF find most important topic(topics) and find all necessary sentences revolving round it using spacy matcher(find patters) --> ALgorithm.
2. Using Gorbid I converted PDF to XML which is saved in xml folder.
3. Using approach in task 1 found contributing sentences
4. Since even contributing sentences have length of about 8000 words used Bigbird Pegasus which can use more than 4000 tokens (unlike 576 in traditional transformer models)
5. Since Summeval have dependency issue for macos and kaggle/Colab I used the original rogue score library https://pypi.org/project/rouge-score/ to find metric of absractive summarization compared to original abstract.

</br>
All contributing sentences/ Rogue Score / Abstractive summarization is saved in csv folder file

## Rogue Score

Final rogue score of bigbird model compared to abstract is 
```
'rouge1': Score(precision=0.4372093023255814, recall=0.42152466367713004, fmeasure=0.4292237442922374)
'rouge2': Score(precision=0.14018691588785046, recall=0.13513513513513514, fmeasure=0.13761467889908258)
'rougeL': Score(precision=0.20465116279069767, recall=0.19730941704035873, fmeasure=0.2009132420091324)}
 ```

 ## Code on Kaggle
 Link : https://www.kaggle.com/code/parthplc/extract-data-from-research-paper-final?scriptVersionId=90756568
 Score Csv Link : https://docs.google.com/spreadsheets/d/1l46_Zg5qS1aCgiTycvRk5EBTkq5tS4RRjnauUv4YOmc/edit?usp=sharing

