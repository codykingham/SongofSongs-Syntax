# SongofSongs-Syntax

This repository contains the iPython notebooks used in my recent thesis, "Clause Syntax in the Song of Songs: A Preliminary Study" (MA Thesis, Southeastern Baptist Theological Seminary, 2016). A copy of the paper can be obtained at https://www.academia.edu/25273297/Clause_Syntax_in_the_Song_of_Songs_A_Preliminary_Study.

The searches make use of the Eep Talstra Centre for Bible and Computer database (ETCBC4b) through LAF-Fabric. 
That database can be accessed at: 
https://github.com/ETCBC

There are three primary directories containing Python code used for the project. 1) NLTK and ETCBC data for English Translation evaluations, 2) a comparison of cola boundaries and syntactic units; cola from BHQ and D. Philip Roberts' 2001 dissertation, "Let Me See Your Form: Seeking Poetic Structure in the Song of Songs." (PhD Dissertation, Westminster Theological Seminary), 3) ETCBC database searches for clause syntax in the Song of Songs along with statistical analyses.

The three datasets are explained and described below:

1. English_Translations
<br>
These notebooks look at the NAS, ESV, NIV, and NLT English translations of the Song of Songs to measure which tenses they select to translate the Hebrew verbs. The data for each of the translation analyses are stored in the respective directories, but NAS is stored in the main English_Translations directory as it serves as the example code. There are two iPython notebooks used for the work. The first, "English_trans_processing.ipynb" produces a simple .txt file in which the English and Hebrew verbs are isolated for each verse so that I could manually compare them faster. NLTK and ETCBC are used to pull the verbs. I manually input the data into a csv file (stored in its respective translation directory). The second notebook, "English_verb_analyses.ipynb" analyzes the csv files to produce statistical results. The data was eventually synthesized into a table and described further in my paper, pp. 13-15.
<br>
<br>
2. Stichometry_vs_Syntax
<br>
These searches aim to answer the following questions: how often do poetic cola agree with clause boundaries? If they do not agree with clause boundaries, what syntactic structure DO they agree with? In the ETCBC database, syntactic structures carry a feature, "monad set" (https://shebanq.ancient-data.org/shebanq/static/docs/featuredoc/features/comments/monads.html). A monad set contains a range of numbers that correspond to individual words. By inputing the monad number of the beginning and ending word for each poetic cola in BHQ and Roberts, I compared the sets to see if they corresponded with data in ETCBC4b. This search was aided by the code stored in the SHEBANQ example notebook "monads.ipynb" (https://shebanq.ancient-data.org/shebanq/static/docs/tools/shebanq/monadsets.html). There are three steps in processing this particular data. 
<br>
<br>
    A. monad_input.ipynb: This step provided a chance to practice Python while building an interactive program to input the beginning and ending monad numbers for each cola. The monad sets are written to a csv file to be processed in step B.
    <br>
    <br>
    B. monad_search.ipynb: This step takes the csv files created in step A and compares the enclosed monad sets with monad sets in the ETCBC database. Syntactic units are stored in a new csv file in an abbreviated form to be analyzed in step C. 
    <br>
    <br>
    C. stichometry_analyses.ipynb: This is the final step and processes the csv file from step B into usable statistics. For monad sets that did not correspond with a formal syntactic unit, code was written to look up every syntactic unit contained so as to determine why these cola did not correspond at all.
<br>
The synthesis of these searches and their effect on my project can be read about in my paper, pp. 35-44.
<br>
<br>
3. Clause_Syntax
<br>
These searches look up and analyze the kinds of clauses in the Song of Songs along with their distribution. There are three notebooks: clause_stats.ipynb provides the basic clause statistic data reflected in p. 45ff in my paper; Song_cl_relations.ipynb looks up the mother-daughter clause relations stored in ETBCB4b and outputs a csv grid containing the relationships; finally, word_order_verbs.ipynb looks at word order in verbal clauses in the Song. It examines the issue from several different perspectives. The purpose and use of this data can be read about further in my paper, pp. 58-60.
