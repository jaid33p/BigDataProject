# BigDataProject

Overview:

The goal of this project is to develop a Classification system for health insurance plans, including Network.csv, PlanAttribute.csv, Business Rules.csv, ServiceArea.csv, Benefits_Cost_Sharing.csv, Rate.csv.They encompass details about various insurance plans, their benefits, costs, provider networks, and plan attributes. The primary aim of the recommendation system is to offer suitable health insurance plans based on user-provided parameters such as health conditions, budget, location, marital status, dependents, and more.

Dataset:

The dataset utilized is named the Health Insurance Marketplace dataset, comprising five tables.


Plan Attributes, the first table, provides details on parameters such as IssuerId, PlanID, Source, Plan Start and Expiration Dates, Guaranteed Rate, NetworkId, and CSRVariation Time, offering comprehensive information about different plan aspects.

Business Rules, the second table, includes parameters such as IssuerID, Source Name, StandardComponent, and rules related to maximum dependents for various family structures, assisting in filtering and identifying the most suitable plans for users based on predefined rules.

Service Area is the third table, including BusinessYear, StateCode, IssuerId, SourceName, VersionNum,ServiceAreaId, ServiceAreaName, CoverEntireState, County, PartialCounty, ZipCodes, PartialCountyJustification, MarketCoverage providing more information on the Service area of the health insurance.

Fourthly, there is Network which contains BusinessYear, StateCode, IssuerId, SourceName, VersionNum, NetworkName, NetworkId, NetworkURL  and MarketCoverage giving more insight into the type of network being used by in which particular business year.

The fifth table, Benefit Cost and Sharing, consolidates benefits based on a common plan ID, featuring parameters such as benefit name, business year, PlanID, IssuerID, LimitQty, and LimitUnit.

The sixth table, Rate, includes parameters like Age, IssuerId, PlanID, StateCode, Tobacco use, and various subscriber and dependent categories, aiding in determining insurance plan rates.



Research Question:

Our objective is to tackle several inquiries to aid in constructing a Classification system and conducting its analysis. Initially, we seek to identify the predominant health insurance plans available in the user's locality. Additionally, we aim to understand how an individual's circumstances influence the cost of their chosen plan. Furthermore, we aim to compare three algorithms for classification and assess their respective performances to determine which one is more suitable for our use case.

Model Class:

We'll employ Random Forest, XGBoosting and Decision Tree algorithms to develop our recommendation system. These algorithms are commonly used to offer personalized suggestions to users. CRandom Forest utilizes an ensemble of decision trees, XGBoost employs gradient boosting techniques, and Decision Trees construct individual trees for classification.

Algorithms:

Random Forest: 
Random Forest is an ensemble learning method that constructs multiple decision trees during training and outputs the mode of the classes (classification) or the mean prediction (regression) of the individual trees. It mitigates overfitting by averaging multiple decision trees, resulting in a more robust and accurate model.

XGBoost: XGBoost, short for Extreme Gradient Boosting, is an advanced implementation of gradient boosting algorithms. It systematically boosts the performance of weak learners (individual decision trees) by optimizing a differentiable loss function through gradient descent. It incorporates regularization techniques to prevent overfitting and achieves state-of-the-art performance on various classification tasks.

Decision Tree:
A decision tree classifier is implemented for predicting health insurance plans based on various features such as state code, source name, tobacco use, age, dependents, and tobacco rate. The dataset is split into training and testing sets using the train_test_split function. The decision tree classifier is trained on the training data using the fit method. Once trained, the decision tree is visualized using the plot_tree, which generates a graphical representation of the decision tree structure. The resulting tree illustrates how the model makes decisions based on the selected features to classify instances into different plan IDs.

References:

1. https://www.kaggle.com/datasets/hhs/health-insurance-marketplace
2. https://www.cms.gov/research-statistics-data-systems/marketplace-products/2022-marketplace-open-enrollment-period-public-use-files


