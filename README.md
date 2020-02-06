# Peer-Reviewed Publication in Stanford's Pacific Symposium of Biocomputing, Waimea, Hawaii (February 2018)

The GeneDive web application enables researchers and clinicians to quickly retrieve gene-gene interactions and to visualize and explore graphical networks of those interactions.  This work was a collaboration between the Departments of Medicine and Genetics at Stanford University, and the Department of Computer Science at San Francisco State University.  

You can access a user-friendly version of the paper [here](https://github.com/pprevide/Stanford-Pacific-Symposium-Of-Biocomputing-paper/blob/master/publication/Previde_GeneDive_2018.pdf), and the version as it appears on the NIH website [here](https://github.com/pprevide/Stanford-Pacific-Symposium-Of-Biocomputing-paper/blob/master/publication/nih_version.pdf).  The PubMed site for the paper is [here](https://www.ncbi.nlm.nih.gov/pubmed/29218917).  

## The GeneDive Application

GeneDive users can search for one or more genes or gene sets, and the application returns all the interactions between the specified genes in tabular and graphical form, along with the information associated with the publication(s) that reported the interaction.  A complete description of the capabilities of GeneDive can be found in the paper.  

![Network Visualization](https://github.com/pprevide/Stanford-Pacific-Symposium-Of-Biocomputing-paper/blob/master/images/gata6.png "Network visualization")

## Analysis of Underlying GeneDive Data
As of the publication date of this paper, GeneDive presented data for over three million gene-gene interactions extracted from biomedical literature.  The literature consisted of 100,000 PLOS articles and 340,000 PMC articles.  One of the analytical tasks of this work was determine the extent to which GeneDive retrieves all of the interactions contained in gene sets curated by research institutions.  As such, the curated gene sets served as a ground-truth, and we computed the precision, recall, and F1 scores associated with the retrieval of these curated gene-gene interactions by GeneDive from PLOS and PMC corpora using Python programming.   Using these computations, we gained insights as to the strengths and weaknesses of the interaction data underlying GeneDive.  The paper provides a complete description of this analysis and its implications.

<p align="center"> (img src="https://github.com/pprevide/Stanford-Pacific-Symposium-Of-Biocomputing-paper/blob/master/images/Table2.png") </p>

<!--At the heart of the extraction process is the DeepDive<sup>1</sup>  text mining system and inference engine, and the application of DeepDive to biomedical literature to extract the interactions in GeneDive is reported in Mallory *et al.*, [here](https://academic.oup.com/bioinformatics/article/32/1/106/1742428). -->  

## Future Work
GeneDive is in active development as of January 2020, and its data have expanded to include gene-drug, gene-disease, and disease-drug interactions as well.  

<sup>1</sup> The DeepDive website can be accessed [here](http://deepdive.stanford.edu/).  DeepDive is no longer in active development and has largely been succeeded by the [Snorkel](https://www.snorkel.org/) system. 
