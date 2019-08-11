# hearthstone-card-package
Revealing hearthstone card packages through unsupervised clustering algorithms.
In Hearthstone, players assemble a deck of 30 cards to play against each other. The fact that some cards synergize well with each other gives rise to the idea of a "package." That is, when considering which card to include in a deck, a set of cards that work really well together should be considered as one bundle, or a cluster.
This project aims to uncover these 'bundles' or 'packages' through clustering cards together based on the vast decklists in Hearthpwn.

### Data source
History of Hearthstone https://www.kaggle.com/romainvincent/history-of-hearthstone/downloads/history-of-hearthstone.zip/3
1. data.csv
2. refs.json

The History of Hearthstone includes:
1. data.csv: scraped data of decks posted on Hearthpwn. Decks are from all expansions up to Mean Streets of Gadgetzan.
2. refs.json: information on all Hearthstone cards such as card ID, name, mana cost, etc.

### Jupyter notebooks:
1. kmeans clustering

### Insights
#### 1. kmeans clustering
