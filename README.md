### Kaggle Competition | [Home Depot Product Search Relevance](https://www.kaggle.com/c/home-depot-product-search-relevance)


### 1. My Conclusion Analysis Report - Jupyter Notebook
* [Home Depot Product Search Analysis](https://github.com/miedlev/Bikesharing-Demend/blob/main/Bikesharing.ipynb)


### 2. About Data :
* This data set contains a number of products and real customer search terms from Home Depot's website. The challenge is to predict a relevance score for the provided combinations of search terms and products. To create the ground truth labels, Home Depot has crowdsourced the search/product pairs to multiple human raters.

The relevance is a number between 1 (not relevant) to 3 (highly relevant). For example, a search for "AA battery" would be considered highly relevant to a pack of size AA batteries (relevance = 3), mildly relevant to a cordless drill battery (relevance = 2), and not relevant to a snow shovel (relevance = 1).

Each pair was evaluated by at least three human raters. The provided relevance scores are the average value of the ratings. There are three additional things to know about the ratings:

* The specific instructions given to the raters is provided in relevance_instructions.docx.
* Raters did not have access to the attributes.
* Raters had access to product images, while the competition does not include images.

Your task is to predict the relevance for each pair listed in the test set. Note that the test set contains both seen and unseen search terms.


### 3. Process Introduction :
It is a competition that can be said to be Kaggle's introductory period and conducts a Python-based analysis. 

**[My focusing was on]** 
1. Correlation coefficient Analysis 
2. Feature engineering
3. Word(search_term, brand name) columns analysis, count, coincidence
3. Relevance analysis strategy
4. Ensemble Model Selection(RandomForestRegressor)
5. 'mean_squared_log_error', 'mean_absolute_error', 'mean_squared_error'  metrics
6. hyperparameter Tuning 


**[Dependencies & Tech]:**
* [IPython](http://ipython.org/)
* [NumPy](http://www.numpy.org/)
* [Pandas](http://pandas.pydata.org/)
* [SciKit-Learn](http://scikit-learn.org/stable/)
* [SciPy](http://www.scipy.org/)
* [Seaborn](https://seaborn.pydata.org/)
* [Matplotlib](http://matplotlib.org/)
* [StatsModels](http://statsmodels.sourceforge.net/)
* [nltk](https://www.nltk.org/)



### 4. Home Depot Product Search Relevance
Shoppers rely on Home Depot’s product authority to find and buy the latest products and to get timely solutions to their home improvement needs. From installing a new ceiling fan to remodeling an entire kitchen, with the click of a mouse or tap of the screen, customers expect the correct results to their queries – quickly. Speed, accuracy and delivering a frictionless customer experience are essential.

In this competition, Home Depot is asking Kagglers to help them improve their customers' shopping experience by developing a model that can accurately predict the relevance of search results.

Search relevancy is an implicit measure Home Depot uses to gauge how quickly they can get customers to the right products. Currently, human raters evaluate the impact of potential changes to their search algorithms, which is a slow and subjective process. By removing or minimizing human input in search relevance evaluation, Home Depot hopes to increase the number of iterations their team can perform on the current search algorithms.
