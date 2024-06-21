<h1><b>Stock Price Forecasting</b></h1>
<hr></hr>
<h5>Name : Shaun Kwo Rui Yu</h5>

<hr></hr>
<h5><b>The objectives of this project are to:</b></h5>
<ol>
<li>Explore the provided dataset and gain insights into its structure and characteristics.</li>
<li>Build time series forecasting models to predict the stock prices of Apple, Amazon, and DBS for the next 60 days.</li>
</ol>

<h5><b>Background Info:</b></h5>
The dataset contains information related to stock prices, including historical prices for Apple, Amazon, and DBS. 
The goal is to develop time series forecasting models that accurately predict stock prices to aid in financial decision-making.

<h5><b>Additional Info:</b></h5>
Stock price forecasting involves predicting future values of a stock based on historical data. This information is crucial for investors and financial analysts to make informed decisions.

Potential Features Influencing Stock Prices:
<ol>
<li>Historical stock prices</li>
<li>Market trends</li>
<li>External factors affecting the stock market</li>
</ol>

<h5><b>Steps in the Project:</b></h5>
<ol>
    <li><b>Step 1: Understanding the Dataset</b>
        <ol>
            <li>1.1 Load the Dataset:
                <ul>
                    <li>Import the necessary libraries (pandas, matplotlib, statsmodels).</li>
                    <li>Load the dataset `CA2-Stock-Price-Data.csv`.</li>
                </ul>
            </li>
            <li>1.2 Exploratory Data Analysis (EDA):
                <ul>
                    <li>Explore the structure of the dataset (columns, data types).</li>
                    <li>Check for missing values and handle them if necessary.</li>
                    <li>Visualize the time series data to understand trends, seasonality, and outliers.</li>
                </ul>
            </li>
        </ol>
    </li>
    <li><b>Step 2: Feature Engineering</b>
        <ol>
            <li>2.1 Data Preprocessing:
                <ul>
                    <li>Convert the date column to a datetime type.</li>
                    <li>Set the date as the index of the DataFrame for time series analysis.</li>
                </ul>
            </li>
        </ol>
    </li>
<li><b>Step 3: Time Series Analysis</b>
    <ol>
        <li>3.1 Augmented Dickey-Fuller Test:
            <ul>
                <li>Apply the Augmented Dickey-Fuller test to check for stationarity in the time series data.</li>
                <li>Check p-values to determine if differencing is necessary.</li>
                <li>Differencing if p-value is much >0.05</li>
            </ul>
        </li>
        <li>3.2 Seasonal Decomposition
            <ul>
                <li>Perform seasonal decomposition to analyze trends, seasonality, and residuals.</li>
                <li>Use techniques like moving averages to smooth out fluctuations.</li>
                <li>Examine decomposed components: trend, seasonality, and residuals.</li>
            </ul>
        </li>
    </ol>
</li>
    <li><b>Step 4: Modelling and Evaluation</b>
        <ol>
            <li>4.1 Train-Test Split:
                <ul>
                    <li>Split the dataset into training and testing sets.</li>
                    <li>Use a significant portion for training to ensure the model captures patterns effectively.</li>
                </ul>
            </li>
            <li>4.2 Build Initial Model:
                <ul>
                    <li>Use the statsmodels library to build an initial ARIMA or SARIMA model.</li>
                    <li>Train the model on the training set.</li>
                </ul>
            </li>
            <li>4.3 Evaluate Initial Model:
                <ul>
                    <li>Evaluate the model's performance on the testing set.</li>
                    <li>Use metrics like Mean Squared Error (MSE) or Root Mean Squared Error (RMSE).</li>
                </ul>
            </li>
        </ol>
    </li>
    <li><b>Step 5: Model Improvement</b>
        <ol>
            <li>5.1 Hyperparameter Tuning:
                <ul>
                    <li>Experiment with different hyperparameters of the time series model.</li>
                    <li>Use techniques like grid search to find optimal hyperparameters.</li>
                </ul>
            </li>
            <li>5.2 Refinement:
                <ul>
                    <li>Refine the model based on the tuning results.</li>
                    <li>Reevaluate the model's performance on the testing set.</li>
                </ul>
            </li>
        </ol>
    </li>
</ol>



<h3>Conclusion</h3>
<ul>
    <li>Summarize key findings, insights, and challenges.</li>
    <li>Provide recommendations for further improvement or exploration.</li>
</ul>
<hr>

<hr></hr>

<h1><b>Student Segmentation Clustering</b></h1>
<hr></hr>


<h5><b>Objectives:</b></h5>
<ol>
    <li>Analyse the dataset `Student_Performance_dataset.csv` with 1000 students' information.</li>
    <li>Group students into clusters to cater to their specific needs.</li>
    <li>Identify groups of students requiring more attention.</li>
</ol>

<h3><b>Background Information:</b></h3>
In education, the focus is on enhancing the learning experience and academic outcomes for students. A sample of 1000 students' data such as age, gender, and subject scores provides a valuable resource for understanding diverse learning needs. The goal is not only to categorize students into clusters but to help students achieve their acedamic goals and also make more personalized and enriching academic experience.

It is also <b>interesting to note</b> that since there is <b>so many different types of genders</b>, this datasets is most probably <b>an american dataset</b></p>

<h5><b>Additional Notes:</b></h5>
<p>Consider the changing landscape of education and the importance of adapting to students' diverse needs.</p>

<h5><b>Steps in the Project:</b></h5>
<ol>
    <li><b>Step 1: Understanding the Dataset</b>
        <ol>
            <li>1.1 Load the Dataset:
                <ul>
                    <li>Import the necessary libraries (pandas, scikit-learn).</li>
                    <li>Load the dataset 'Student_Performance_dataset.csv'.</li>
                </ul>
            </li>
            <li>1.2 Exploratory Data Analysis (EDA):
                <ul>
                    <li>Explore the structure of the dataset (columns, data types).</li>
                    <li>Check for missing values and handle them if necessary.</li>
                    <li>Visualize key features to understand student distribution.</li>
                </ul>
            </li>
        </ol>
    </li>
    <li><b>Step 2: Background Research & Data Exploration</b>
        <ol>
            <li>2.1 Data Exploration:
                <ul>
                    <li>Visualize the distribution of age, gender, and subject scores.</li>
                    <li>Identify any patterns or trends in the student data.</li>
                </ul>
            </li>
        </ol>
    </li>
    <li><b>Step 3: Feature Engineering</b>
        <ol>
            <li>3.1 Preprocess Data:
                <ul>
                    <li>Handle categorical features (e.g., gender) using encoding.</li>
                    <li>Standardize numerical features (e.g., age, scores) for uniformity.</li>
                </ul>
            </li>
        </ol>
    </li>
    <li><b>Step 4: Modelling and Evaluation</b>
        <ol>
            <li>4.1 Build Initial Model:
                <ul>
                    <li>Apply k-means clustering algorithm to the preprocessed data.</li>
                    <li>Examine the resulting clusters and their characteristics.</li>
                </ul>
            </li>
            <li>4.2 Evaluate Initial Model:
                <ul>
                    <li>Assess the performance of the model based on relevant metrics.</li>
                    <li>Consider silhouette score or other clustering evaluation metrics.</li>
                </ul>
            </li>
        </ol>
    </li>
    <li><b>Step 5: Model Improvement</b>
        <ol>
            <li>5.1 Experiment with k:
                <ul>
                    <li>Test the clustering algorithm with different values of k.</li>
                    <li>Explore the impact of changing the number of clusters.</li>
                </ul>
            </li>
            <li>5.2 Refinement:
                <ul>
                    <li>Adjust hyperparameters or preprocessing steps based on evaluation results.</li>
                    <li>Reevaluate the model's performance after refinement.</li>
                </ul>
            </li>
        </ol>
    </li>
</ol>


