# Anonymization Algorithms for Privacy-Sensitive Networks
[comment]: <This is a master's thesis project, which includes 5 methods for graph anonymization by edge deletion. More details of algorithms can be found in the [corresponding thesis]() in the [repository of LIACS]().> 

## Dependencies
iGraph  
NetworkX  
NumPy  
Pandas  
scikit-learn  
Matplotlib  

## Data
Five datasets are used in this project:

* [Copenet SMS, Copenet FB](https://figshare.com/articles/dataset/The_Copenhagen_Networks_Study_interaction_data/7267433/1?file=13389839)
* [CollegeMsg](http://snap.stanford.edu/data/CollegeMsg.html)
* [ca-GrQc](http://snap.stanford.edu/data/ca-GrQc.html)
* [ego Facebook](http://snap.stanford.edu/data/ego-Facebook.html)

## Usage
For (n,m)-anonymity, the code can be executed directly. For d-k-anonymity, this code builds upon the work of de Jong Rachel et al. [1]. Therefore, first, it is necessary to follow the instructions [here](https://github.com/RacheldeJong/dkAnonymity). Afterward, place the `Anonymization-iGraph.ipynb` in the nauty directory (nauty27r3).

## Reference
[1] Rachel G. de Jong, Mark P. J. van der Loo, and Frank W. Takes. 2023. Algorithms for Efficiently Computing Structural Anonymity in Complex Networks. ACM J. Exp. Algor. 28, 1, Article 1.7 (August 2023), 22 pages. https://doi.org/10.1145/3604908
