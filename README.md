# CloudLab Analysis

This github repository contains the source code of analytical programs that analyze research trends and topics in research projects done on [CloudLab](www.cloudlab.us). To accomplish this goal, these programs utilize natual language processing, topic modelings, and other machine learning methods. 

# Data

Data (publications, online groups, emails contents) are stored on a Goole Drive (private to group members). A configuration file (gitignored) needs to be setup inside the cloned repository to point to Google Drive's locations on individual members' computing platform. 


# Environment

To set up the environment, latest version of Anaconda 2 is needed. Inside Anaconda Navigator, the new environment uses Python 2.7. The following libraries are needed:

pdfminer
```
  conda install -c conda-forge pdfminer
```

nltk
```
  conda install -c anaconda nltk 
```

gensim
```
  conda install -c anaconda gensim 
```

spacy
```
  conda install -c spacy spacy
  python -m spacy.en.download
```

pyldavis
```
  pip install pyldavis 
```
*For **pyLDAvis**, also make the following modifications to the class **NumPyEncoder** in PATH-TO-ANACONDA/envs/YOUR-ENV-NAME/lib/site-packages/pyLDAvis/utils.py:* 
```
  if np.iscomplexobj(obj):
    return abs(obj)
```

matplotlib
```
  pip install matplotlib
```

sbs
```
  pip install seaborn
```
