# SongofSongs-Syntax

This repository contains the iPython notebooks used in "Clause Syntax in the Song of Songs: A Preliminary Study."

A copy of the paper can be obtained at https://www.academia.edu/25273297/Clause_Syntax_in_the_Song_of_Songs_A_Preliminary_Study.

The searches make use of the Eep Talstra Centre for Bible and Computer database (ETCBC4b) through LAF-Fabric. 
That database can be accessed at: 
https://github.com/ETCBC

There are three primary directories containing Python code used for the project. 1) NLTK and ETCBC data for English Translation evaluations, 2) a comparison of cola boundaries and syntactic units; cola from BHQ and D. Philip Roberts' 2001 dissertation, "Let Me See Your Form: Seeking Poetic Structure in the Song of Songs." (PhD Dissertation, Westminster Theological Seminary), 3) ETCBC database searches for clause syntax in the Song of Songs along with statistical analyses.

The three datasets are explained and described below:

1. English_Translations
<br>
These notebooks look at the NAS, ESV, NIV, and NLT English translations of the Song of Songs to measure which tenses they select to translate the Hebrew verbs. The data for each of the translation analyses are stored in the respective directories, but NAS is stored in the main English_Translations directory as it serves as the example code. There are two iPython notebooks used for the work. The first, "English_trans_processing.ipynb" produces a simple .txt file in which the English and Hebrew verbs are isolated for each verse so that I could manually compare them faster. NLTK and ETCBC are used to pull the verbs. I manually input the data into a csv file (stored in its respective translation directory). The second notebook, "English_verb_analyses.ipynb analyzes the csv files to produce statistical results. The data was eventually synthesized into a table and described further in my paper, "Clause Syntax in the Song of Songs" (13-15).

2. Stichometry_vs_Syntax
<br>
These searches aim to answer the following questions: how often do poetic cola agree with clause boundaries? If they do not agree with clause boundaries, what syntactic structure DO they agree with? There are three steps in processing this particular data. 
<br>
    A. 
