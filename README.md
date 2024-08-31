# Real-Estate-Price-Predictor
**Project Overview**: 

**Introduction**
The "Real Estate Price Predictor" project aimed to develop a machine learning model for real estate prices concerning various features such as but not limited to location and square footage, number of bedrooms, etc. To that effect, the project encompasses backend model development and shares a front-end interface which the user can interact with to retrieve predictions.

**Key Components**:

1. `bhp.ipynb` Jupyter Notebook:
- **Purpose:** The following Jupyter Notebook is the development environment of the machine learning model. Normal procedures that are included in this documentation is described below:
     - **Data Analysis:** Preliminary studies on the data set for a better understanding of the structuring, distribution, and relationships of features.
Feature Engineering: This will also accompany the process of converting raw data into an operable format, which might include imputations for missing values, encoding on categorical variables, and scaling on numerical features. 
 Model Training: The process would also involve training-from simple linear regression to using decision trees to complex models to know the trends within the dataset.
Model Evaluation: This shall be done through the use of R-squared, Mean Absolute Error among others in assessing model performance. Ensuring that the model will generalize well on new data is the reason behind this. Selection of the final model: After trying many models and hyperparameters, the best performing model shall be selected and saved.

2. banglore_home_prices_model.pickle:
- **Purpose:** This stores a serialized version of the trained machine learning model. Its format is such that it can be loaded with ease and then subsequently used to make predictions. The model has only been trained with Bangalore's real estate data, and hence, it can make price predictions keeping in view the local market trends.

3. **Python Script `server.py`:
- **Objective:** It hosts the web application and usually uses any framework like Flask or Django. It will receive a request from any user interested in the price prediction of any particular estate.
Working: In the case of an incoming user feeding in an input about the location, area, and number of bedrooms of his house, then the server uses the model loaded from the file `banglore_home_prices_model.pickle` to return a predicted price corresponding to the user's provided data.

4. **Front-end Files:**
- **`app.html`:** Provides the skeleton of the web page. It also carries the forms that take user inputs. For example, dropdowns for location and text fields for square footage.
- **`app.css`:** Beautifies the web page so it's pleasing to the user's eye and easy to use.
- **`app.js:`** it makes the web page interactive. This way, it can take user input and send it to the server and show the returned prediction.
5. **`columns.json`: **
• **Purpose:** This is probably a list of what features were used in the model; for example, location, number of bedrooms. When data is input through the frontend, that server will want to map that onto the right features used during training in the model. 
• **Functionality:** Ensuring that whatever data is fed into the model to make a prediction went through the same preprocessing steps as the training data did.

**General Project Purpose**:
The project aims at developing some sort of practical tool for house price prediction. By applying historical data and machine learning methods, one can develop an approximate price of this or that particular property when its characteristics get fed into the model. To this end, the work could be really useful for real estate professionals, buyers, or sellers in making a good choice within the market.

It's a tool wherein backend machine learning has been integrated into a non-technical, user-friendly web interface for accessibility by non-technical users so that advanced predictive analytics can be used sans deep understanding of the algorithms.
