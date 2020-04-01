# hearthstone-card-package
Revealing hearthstone card packages through unsupervised clustering algorithms.
In Hearthstone, players assemble a deck of 30 cards to play against each other. The fact that some cards synergize well with each other gives rise to the idea of a "package." That is, when considering which card to include in a deck, a set of cards that work really well together should be considered as one bundle, or a cluster.
This project aims to uncover these 'bundles' or 'packages' through clustering cards together based on the vast decklists in Hearthpwn.  

## Uses
With a reliable and effective tool to identify card packages, it may be possible to employ such clustering algorithms to help deck building in the future using up-to-date data. Possible uses include optimizing current decks archetypes, coming up with new ones, or identifying emerging metagame trends.

## Data source
History of Hearthstone https://www.kaggle.com/romainvincent/history-of-hearthstone/downloads/history-of-hearthstone.zip/3
1. data.csv
2. refs.json

The History of Hearthstone includes:
1. data.csv: scraped data of decks posted on Hearthpwn. Decks are from all expansions up to Mean Streets of Gadgetzan.
2. refs.json: information on all Hearthstone cards such as card ID, name, mana cost, etc.

## Jupyter notebooks:
1. KMeans clustering: `hs-package-kmeans`
2. PCA for data visualization: 

## High-level insights
### 1. KMeans clustering
From the notebook `hs-package-kmeans`, we can see that KMeans clustering works sufficiently well at identifying card packages. Many sets of cards vital to the strong decks in the metagame at that time were identified as a cluster. For instance, a highly optimized **Freeze Mage** archetype is infamously rigid with little room for card changes. The core cards are identified in the **Freeze Mage** cluster. Still, KMeans Clustering does not allow one card to be a member of multiple clusters. Hence, other clustering algorithms may need to be brought in to reflect different archetypes within a class that may utilize the same few cards.
### 2. Principal Component Analysis (PCA)
This section explores visualization of the cards and where they stand relative to one another using Principal Component Analysis (PCA). PCA decomposes a multi-dimensional matrix of features into a number of arbitary axes which explain the largest portion of the samples' variance. For visualizations, PCA is generally used to decompose the features into 2 dimensions and the samples are then plotted using this 2-dimensional coordinate system.  
From the notebook, 
