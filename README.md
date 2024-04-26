# CHEME 4/5800 Parts of Molecule Tagging Project
Template repository for the CHEME 1800/4800 parts of a molecule tagging problem. 

## Description
One of the challenges of working with online reaction databases, e.g., KEGG, is dirty data, i.e., mistakes in the reaction records in the online database. 
Design and implement a program that identifies unbalanced reaction strings. This program should consist of three components. 
* First, we must interface with the KEGG Application Programming Interface (API) to pull down reaction data. Information on the [KEGG API can be found here](https://www.kegg.jp/kegg/rest/).
* Next, you’ll tokenize chemical formula strings in a reaction string to produce a composition dictionary for each compound. The composition dictionary has elements as keys and the number of that element as the value. For example, C6H12O6 would give C=> 6, H=>12, and O=> 6. Example reaction data is included in the [e_coli_core.json file](data/e_coli_core.json), which was taken from the [Core E. Coli model of Palsson and coworkers](https://systemsbiology.ucsd.edu/Downloads/EcoliCore).
* Finally, use the composition dictionaries to tell the user if a chemical reaction is balanced. If the reaction is unbalanced, it will return which elements are incorrect and by how much. Test your project on datasets with known errors and then on unseen data.
