# Cognizant-Artificial-Intelligence-Virtual-Experience

### Task 1 - Exploratory Data Analysis
Conduct analysis on your client's sample sales dataset and identify customer behaviours to generate insights and provide commercial recommendations.

#### Background information for the task
Gala Groceries is a technology-led grocery store chain based in the USA. They rely heavily on new technologies, such as IoT to give them a competitive edge over other grocery stores. They pride themselves on providing the best quality, fresh produce from locally sourced suppliers. However, this comes with many challenges to consistently deliver on this objective year-round.

Gala Groceries approached Cognizant to help them with a supply chain issue. Groceries are highly perishable items. If you overstock, you are wasting money on excessive storage and waste, but if you understock, then you risk losing customers. They want to know how to better stock the items that they sell. This is a high-level business problem and will require you to dive into the data in order to formulate some questions and recommendations to the client about what else we need in order to answer that question.

#### Main goals of this task are :
1. Summarize the findings and provide some suggestions as to what else is needed to fulfill their business problem
2. Draft an email containing this information to the Data Science team leader to review.

#### Trends and Insights
1. Fruit & vegetables are the 2 most frequently bought product categories.
2. Non-members are the most frequent buyers within the store.
3. Cash is the most frequently used payment method.
4. 11am is the busiest hour with regards to number of transactions.

#### Views and Recommendations
1. This is a very broad statement and in order to tackle this with better accuracy, we need to identify a specific problem statement that the business would like to solve. For example, can we predict the demand of products on an hourly basis in order to procure products more intelligently?
2. We need more data. The current sample only covers 7 days and 1 store.
3. Based on the problem statement that we move forward with, we will need more datasets to help describe the outcome that we’re trying to model. For example, if we’re modeling demand for products, we may want to include information about stock levels or weather conditions. 

#### Submitted Work
[Task 1: Python EDA](https://github.com/carolinasibrian/Cognizant-Artificial-Intelligence-Virtual-Experience/blob/9077b41a4965ac408e4afa6d4fb286e54f487d77/Task1.ipynb)

[Email Submission](https://github.com/carolinasibrian/Cognizant-Artificial-Intelligence-Virtual-Experience/blob/9077b41a4965ac408e4afa6d4fb286e54f487d77/Email%20template%20(1).docx)

---

### Task 2 - Data Modeling
Extend your analysis from Task 1 to help you predict the stock levels of products based on sales data and sensor data.

#### Background Information for the task
Gala Groceries want to focus on the following problem statement:

“Can we accurately predict the stock levels of products based on sales data and sensor data on an hourly basis in order to more intelligently procure products from our suppliers?” 

The client has agreed to share more data in the form of sensor data. They use sensors to measure temperature storage facilities where products are stored in the warehouse, and they also use stock levels within the refrigerators and freezers in store. 

#### Data Model

<img width="950" alt="Screenshot 2023-06-14 at 6 44 33 PM" src="https://github.com/carolinasibrian/Cognizant-Artificial-Intelligence-Virtual-Experience/assets/130473935/66550b0d-6e74-4af6-8bee-182655c68bde">

#### Main goals of this task are :
1. Based off the data model diagram decide on what data you’re going to use from the data available.
2. Create a strategic plan to answer the problem statement. 
3. Summarize your choices and plan of work in a PowerPoint presentation.

#### Strategic Plan
* Data Model - All the data in the 3 tables will be used
* Plan of Work
   * Data Preparation - Use the data model to merge the data, then clean the data and remove any outliers
   * Feature Engineering - Create new features and transform the dataset ready for predictive modelling
   * Model Experimentation - Testing algorithms with cross-validation
   * Evaluation of results and iteration - Measuring performance metrics
   * Development of product algorithm - Production of the algorithm and an API
   * QA and DevOps - To ensure the model is performing as expected and to integrate the model

#### Submitted Work
[PowerPoint Slide](https://github.com/carolinasibrian/Cognizant-Artificial-Intelligence-Virtual-Experience/blob/1a658577207c6dba40198eeb27829437d802d394/Plan%20(1).pptx)

----

### Task 3 - Model Building and Interpretation
Building a predictive model and interpreting the results back to the business

#### Background Information for the task

The client has provided 3 datasets, transform and model these datasets in a suitable way to answer the problem statement that the business has requested. 

Most importantly, once the modeling process is complete, communicate your work and analysis in the form of a single PowerPoint slide, so that we can present the results back to the business. 

#### Main goals of the task are:
1. Transform and model these datasets
2. Communicate analysis in the form of a single PowerPoint slide

#### Summary
* More Data is required
   * Approximately 50% accuracy with the current set of data and features that were created. In order to test this model for production, we need larger samples
* Price is important
   * Price was an important feature in the model, but the category was not. Are there more features about the products that we can use to include in the model?
* Build on IoT
   * Temperature was also significant within the model, with more IoT data across a larger time period, we believe the accuracy of this model will increase. It also opens up the potential to use open-source data, such as weather. 

#### Submitted Work
[Task 3: Python Modeling](https://github.com/carolinasibrian/Cognizant-Artificial-Intelligence-Virtual-Experience/blob/01f6e2f0bc58316b56a78c429f8ba72035f1cac9/Task3_modeling.ipynb)

[Powerpoint Slide](https://github.com/carolinasibrian/Cognizant-Artificial-Intelligence-Virtual-Experience/blob/f9b7709554a2a5e0fc1312154ca52c8e1a32aa93/Plan%20(2).pptx)

----
#### Task 4 - Machine Learning Production
Developing machine learning algorithms for production

#### Background Information for the task
Gala Groceries saw the results of the machine learning model as promising and believe that with more data and time, it can add real value to the business.

To build the foundation for this machine learning use case, they want to implement a first version of the algorithm into production. In the current state, as a Python notebook, this is not suitable to productionize a machine learning model. 

Therefore, as the Data Scientist that created this algorithm, prepare a Python module that contains code to train a model and output the performance metrics when the file is run. 

#### Main goals of the task are:
1. Prepare a Python module

#### Submitted Work

[Python Module](https://github.com/carolinasibrian/Cognizant-Artificial-Intelligence-Virtual-Experience/blob/22896526ff4a8cf248fb711bf1208a82e775f03c/task4.py)

----
#### Task 5 - Quality Assurance
Evaluating the production machine learning model to ensure quality results

#### Background Information for the task

The ML engineering team has taken your Python module and deployed the algorithm into production along with the DevOps, which is great!

The DevOps team has been collecting some predictions from the algorithm and has provided these to the ML engineering team, who have performed some testing of the predictions against the actual results for ‘estimated_stock_pct’. The ML engineering team were testing the predictions vs actual results to see how well the algorithm is performing on “live” data.

After performing the tests, the ML engineering team wants to discuss with you some questions about the algorithm in order to further improve the model before the DevOps team integrates it with Gala Groceries’ live system.

#### Main goals of the task are:
1. Discuss some questions about the algorithm 

#### Questions:
1. The accuracy of the predictions about the live data are not as good as the results that you showed during the training of the model. Why do you think this is? - **The model is underfit**
2. Can you suggest a way to improve the predictions on the live data? - **Collect more rows of data to train the model with**
3. The client has offered some additional datasets that may be useful. Can you let us know which two datasets you think would be best to include in the model? - **Weather, deliveries**
4. We would like to explore the possibility of using a more complex machine learning algorithm to see how it compares to the current Random Forest. Can you suggest one to try? - **Neural Network**
5. What would be a disadvantage of using the more complex model from the previous question, against the current Random Forest? - **More difficult to explain the algorithms results**
6. Can you suggest a way that we can optimize the performance of the current Random Forest algorithm? In particular, we want to know how we can improve the MAE of the current algorithm. - **Tune hyperparameters**

----

# [Certificate](https://forage-uploads-prod.s3.amazonaws.com/completion-certificates/Cognizant/5N2ygyhzMWjKQmgCK_Cognizant_p6zCfyAog39HPazpa_1685731949813_completion_certificate.pdf)
