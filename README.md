# spelling-correction
Spelling Error Correction based on Noisy Channel Model 

This is a mini project completed in March 2020 for Introduction to Information Retrieval Course in Bogazici University.

Damerau-Levenshtein edit distance was used and results are reported with and without add-1 smoothing (Laplace smoothing with &#945;=1)

Corpus is taken from [Peter Norvig’s website](http://norvig.com/big.txt)

Author: Mansur Yeşilbursa

This program uses following packages:
os
string
re
time
numpy
math
matplotlib
sys
pandas
seaborn

spelling_correction.py should be placed in a folder that is a subdirectory of the folder that contains
all the other files. (datasets, test sets etc.) 

For example:

Directory for datasets:
/home/mansur/assignment/

Directory for python script:
/home/mansur/assignment/spelling_correction/

You will find additional files accompanying Python script: 
(bigram.npy, character.npy, corpus_prob_list.txt, corpus_word_list.txt) Those files contain preprocessing of 
datasets that are saved in order to reduce run time. They also need to be placed with datasets. (one folder
above the Python script). You can delete those preprocessed files or leave it as it is, however, if you
delete them, the program takes longer to finish. The program would work either way.
You can also specify test sets in the command line. If you don't, the program automatically tries to load test 
sets given in the assignment. (test-words-misspelled.txt and test-words-correct.txt)  

For example:

`python spelling_correction.py error_file.txt correct_file.txt`

OR

`python spelling_correction.py test-words-misspelled.txt test-words-correct.txt`

IS EQUIVALENT TO

`python spelling_correction.py`

