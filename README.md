# WebScrapping - Filmography
Using Selenium WebDriver in Microsoft Edge, the web scraping script automatically extracts Leonardo DiCaprio's movie titles from IMDb. The first step is to open the IMDb homepage, type in "Leonardo DiCaprio," and then select the "People" section.   In order to manage dynamic content, the script scrolls and verifies and clicks on the element and retrieves the movie title from the sibling element that comes before it; if it is "false," it retrieves the title directly. To ensure reliable website engagement and effective data gathering, extracted titles are compiled into a list and saved to a CSV file.   Moreover, the script handles errors and cleans up resources by terminating the WebDriver session at the end.
The same is tried using BeautifulSoup and chrome driver as well.


# Kepler-dataset-Classification
Various ML classification models are experimented upon

The Kepler dataset originates from the Kepler space telescope mission, which was launched by NASA with the primary goal of 
discovering Earth-like planets orbiting other stars. The telescope monitored the brightness of over 150,000 stars to detect 
periodic dips in brightness caused by planets transiting (passing in front of) their host stars.

1.Why did you choose the particular algorithm?  
For all the four algorithms I used, I went into the unique features each algorithm holds and it includes the following:  
For binary classification issues, logistic regression is a useful foundational model. It can be used to determine the probability that a data point belongs to a particular class and is easy to use, interpret, and generate classification probabilities.   An ensemble learning technique for classification is Random Forest algorithm that combines predictions from multiple decision trees to improve performance minimizes overfitting brought on by the usage of several decision trees made from random subsets of the provided data. A majority voting system that uses decision trees for bagging as well. They can generate feature significance ratings and handle both numerical and categorical features.   Support vector machines, or SVMs, are helpful when there are more dimensions than samples and are efficient in high-dimensional spaces. Additionally, they function best when there is a distinct boundary between the classes.   K-Nearest Neighbours, is a straightforward method that performs admirably on small to medium-sized datasets. It works well when the decision boundary is irregular and makes no assumptions about the distribution of the underlying data.

2.What are the different tuning methods used for the algorithm?  
Logistic Regression - Regularization parameters (L1, L2)   
Random Forest Classification - n_estimators, max_depth(expanded until all leaves are pure)   
SVM - Regularization parameter (C), kernel type(default = "rbf")  
KNN - Number of neighbors(default = 5), distance metric (Euclidean, Manhattan, Minkowski(default))  

3.Did you consider any other choice of algorithm?Why or why not?  
All the above four are the algorithms that I considered for this dataset classification.

4.What is the accuracy?  
The models include:   
Logistic regression - 96% accuracy,   
Random Forest Classification - 93% accuracy,   
Support Vector Machine - 97% accuracy,   
K-Nearest Neighbors - 91% accuracy  
All the model accuracies fall above 90% indicating it to be suitable models for this dataset. But with ceratain differences,  
SVM and LR tend to be the best among all the four models.  

5.What are the different types of metrics that can be used to evaluate the model?  
Accuracy, Precision, Recall and F1-score were analyzed.

