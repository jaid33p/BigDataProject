# BigDataProject

OVERVIEW:

Mid-East Canadian Pharmaceutical (MECP) is a company in the medical sector that specializes in offering cold supply chain solutions for medical equipment to various entities. With an extensive inventory of over 508,000 medical products, their goal is to use publicly available data from their suppliers to identify in-demand medical products at specific times throughout the year. They aim to develop a training model using existing data to forecast periods of increased demand for specific medical products. This predictive capability allows them to proactively stock these products before the demand rises, ensuring timely availability and efficient supply chain management.



Dataset:

Based on the details provided by MECP, the dataset requires scraping from the internet using a crawler script. Initially, the dataset comprises the following fields:


 Name (varchar): Product name.
 Description (varchar): Product description.
 Catalogue Number: Unique identifier for the product in the catalogue.
 Price (float): Product price.
 Availability (varchar): Availability status of the product.
 Manufacturer Number (int): Identifier for the manufacturer of the product.
 Invoice Description (varchar): Description of the product on the invoice.
 Feature Property (varchar): Specific features of the product.
 Sterility (bool): Sterility status of the product.
 Link (varchar): URL link for more information about the product.
 Brand Name (varchar): Brand name associated with the product.
 Outer Diameter (float): Outer diameter measurement of the product.
 Needle Length (float): Length of the needle.
 Volume (float): Volume measurement of the product.
 Color (varchar): Color of the product.
 Inner Diameter (float): Inner diameter of the product.
 Size (varchar): Size specification of the product. 
 Age (datetime): Age-related information (e.g., expiration date).
 Shape (varchar): Shape of the product. 
 Catheter Length (float): Length of the catheter (if applicable).
 Composition Ingredient (varchar): Composition or ingredients of the product.

Some of the parameters which are most relevant in are Price, Manufacturer Number, Feature Property, Sterility, Outer Diameter, Needle Length, Color, Size, Age, Catheter Length and Composition Ingredient as these likely to be those that provide meaningful insights into factors affecting product availability.


Research Question:

 	
As per MECP's specifications, the primary objective is to develop a predictive model that can accurately pinpoint times when shortages of medical products are likely to occur. In simpler terms, they aim to use data and analysis to anticipate when there might be a lack of specific medical items, helping them proactively manage their inventory and ensure timely availability of essential products.


Model Class:

As per the outlined specifications, our approach entails utilizing supervised learning models for the training process. This decision is motivated by the need to identify patterns that signal when a product becomes unavailable and to ascertain the particular days of the year when such occurrences are most likely. The goal is to leverage these models to enhance the ability to predict and manage stockouts effectively.



Algorithms:

•	Random Forest: 

Random Forest is an ensemble learning algorithm that builds multiple decision trees during training and combines their predictions to produce a more accurate and robust result. In predicting shortage periods of medical products using the provided dataset, a Random Forest model is trained on product features like price, manufacturer details, and feature properties. After preprocessing and tuning, the model identifies patterns associated with product availability. Feature importance analysis helps pinpoint critical factors affecting shortages. Evaluation focuses on metrics like accuracy and recall to minimize false negatives. Time series considerations may be integrated to capture temporal patterns effectively. Overall, the Random Forest model accurately predicts shortage periods based on the dataset's information. 


•	Gradient Boosting: 

Gradient Boosting algorithms, including popular implementations like XGBoost and LightGBM, offer powerful predictive modeling capabilities. In predicting shortage periods of medical products, Gradient Boosting models, such as XGBoost or LightGBM, are trained on the dataset's product features. These include description, volume, and product properties. Following preprocessing and hyperparameter tuning, the model learns complex relationships in the data to identify patterns associated with product availability. Feature importance analysis aids in understanding key predictors of shortages. Evaluation focuses on metrics like accuracy and recall, with an emphasis on minimizing false negatives. Time series considerations can be incorporated for capturing temporal patterns effectively. Ultimately, Gradient Boosting models provide accurate predictions of shortage periods based on the dataset's information.

