## Dependencies
* [iGraph](https://igraph.org/): 0.10.4
* [NetworkX](https://networkx.org/): 2.8.4
* [NumPy](https://numpy.org/doc/stable/): 1.23.3
* [Pandas](https://pandas.pydata.org/): 1.4.4
* [scikit-learn](https://scikit-learn.org/stable/):1.2.1
* [Matplotlib](https://matplotlib.org/): 3.5.3  

## Data
Five datasets are used in this project:

* [Copenet SMS, Copenet FB](https://figshare.com/articles/dataset/The_Copenhagen_Networks_Study_interaction_data/7267433/1?file=13389839)
* [CollegeMsg](http://snap.stanford.edu/data/CollegeMsg.html)
* [ca-GrQc](http://snap.stanford.edu/data/ca-GrQc.html)
* [ego Facebook](http://snap.stanford.edu/data/ego-Facebook.html)

## Usage
For *(n,m)-anonymity*, the code can be executed directly. For *d-k-anonymity*, this code builds upon the work of de Jong Rachel et al. [1]. Therefore, first, it is necessary to follow the instructions [here](https://github.com/RacheldeJong/dkAnonymity). Afterward, place the `Anonymization-iGraph.ipynb` in the nauty directory (nauty27r4).   

The variable `STEP` refers to the recompute gap *g*, which determines how many edges to be deleted before recomputing the uniqueness. The variable `CALCULATE_TIME` refers to the iteration time. Five anonymization methods are executed by the following functions:   
* random edge deletion: `random1Round`
* degree-based deletion: `max1Round`
* UA-based deletion: `UA1Round`
* LR-based deletion: `LR1Round`
* *(n,m)*-greedy deletion: `greedy1Round`

The training data of LR-based deletion can be found [here](training_data.csv). More details of the algorithms can be found in the corresponding thesis.

## Reference
[1] Rachel G. de Jong, Mark P. J. van der Loo, and Frank W. Takes. 2023. Algorithms for Efficiently Computing Structural Anonymity in Complex Networks. ACM J. Exp. Algor. 28, 1, Article 1.7 (August 2023), 22 pages. https://doi.org/10.1145/3604908
