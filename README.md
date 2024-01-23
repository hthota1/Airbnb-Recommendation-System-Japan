# Airbnb Recommendation System - Japan

![Airbnb image](https://cdn.i.haymarketmedia.asia/?n=campaign-asia%2Fcontent%2FAirbnb-girls-trip.jpg)

# Business Problem

The business problem is two fold. First, Airbnb aims to enhance its presence in Japan by identifying popular properties in Tokyo and expanding its business to other cities outside the capital. Airbnb wants to understand the key factors that contribute to the popularity of properties in Tokyo. These were assessed based on property type, price per night, amenities offered, and user ratings.

Second, Airbnb wants to increase the utilization of the existing housing on the platform. To aid with this, I developed a recommendation system to guide new users in rating properties and receive tailored recommendations based on their preferences.

# Data Overview
* **Datasets:** 
    * Listings provides information on the attributes of the property.
    * Reviews provides information of the user review for the property.
* **Source:** [Inside Airbnb](http://insideairbnb.com/get-the-data)

* **Limitations**
    * User reviews can be biased. Some guests may be more likely to leave reviews based on extreme experiences (either very positive or very negative), leading to a potential bias in the sentiment of reviews
    * Limited historical data due to Covid-19 impact on bookings
    * Listings information can vary in quality. Some listings may have high-quality descriptions and images, while others may lack important details.
* **Filters**
    * Listings with a minimum of 10 reviews
    * May 1, 2023


# Modeling

In the pursuit of creating an effective recommendation system for my Airbnb analysis project, I explored several models:
* KNN Baseline
* KNN Basic
* SVD (Singular Value Decomposition)
* NMF (Non-negative Matrix Factorization)

After fine tuning, the SVD model emerged as the best one, achieving the lowest Root Mean Squared Error (RMSE) at 0.096. Consequently, SVD has been identified as the primary model for the recommendation system, promising personalized suggestions and enhance user experience.

# Recommendations

- **Invest** in entire homes or apartments , for consistent high ratings
- **Include** popular amenities - security, safety features and bath and kitchen essentials
- **Price** the listing under $200/night

# Next Steps

- **Compare** Airbnb market in Tokyo with other major cities to identify unique trends and common patterns 
- **Add** demographic data for reviewers
- **Develop** predictive models to forecast future demand for Airbnb listings

# For more information
The complete analysis can be found in my [Jupyter Notebook](https://github.com/hthota1/Airbnb-Recommendation-System-Japan/blob/main/airbnb_analysis.ipynb) and [presentation](https://github.com/hthota1/Airbnb-Recommendation-System-Japan/blob/main/Presentation.pdf). 

For any additional questions, you can contact me:


**LinkedIn:** linkedin.com/in/harshithathota/

**Email**: harshitha.thota@gmail.com

# Repository Structure
├── data		 				           	 	<- Data files used in this project 

├── images		                         	 	<- Contains images and graphs used in this project sourced from code and outside source

├── .gitattributes		                 	 	<- To track Data file using LFS

├── .gitignore                     	 			<- Contains a list of files to be ignored from Github

├── presentation.pdf		                	<- PDF version of the project presentation

├── README.md 			                      	<- The top-level README for reviewers of this project

└── airbnb_analysis.ipynb 			          	<- Narrative documentation of the analysis in a Jupyter notebook 
