# NLP Annotation Project

This is a semester-long group annotation project in INFO 159. In this project, our group chose Amazon PC Product Reviews as our data and manually annotated the degree of constructiveness of 1000 product reviews. There are three members in our group, and we splitted the labor such that two of us are independent annotator and the third adjudicates any disagreement to produce the final label. While two annotators annotate the dataset independently, we also calculated inter-annotator agreement rate to have a sense of the level of agreement between random annotators. After evaluating the entire dataset with adjudicated labels, we built a classifier to automatically predict our annotated labels. Specifically, we implemented a logistic regression classifier as our baseline model, and tried out Sentence MEMM and BERT, where the latter gives the highest classification accuracy. 
