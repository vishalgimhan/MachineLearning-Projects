# Machine Learning Projects

**1. Waiter Tip Prediction Model**

- **Data Overview**: It includes an initial examination of the waiter tips dataset, showcasing the first few entries and the structure of the data.

- **Data Visualization**: The project presents various scatter plots and pie charts to analyze the relationship between total bill, tips, and other variables like day, sex, time, and smoker status.

- **Data Transformation**: Categorical variables such as sex, smoker, day, and time are transformed into numerical values for further analysis.

- **Model Building**: A Linear Regression model is constructed using features like total bill, sex, smoker, day, time, and size to predict the tip amount.

- **Model Evaluation**: The model’s performance is assessed using the mean squared error metric.

- **Application Development**: A simple application is built to predict the tip amount based on user input for different features.

**2. Future Sales Prediction Model**

- **Data Loading**: It involves importing libraries and loading a dataset from a CSV file into a pandas DataFrame.

- **Data Preprocessing**: Checking for null values in the dataset to ensure data quality.

- **Data Visualization**: Creating scatter plots to visualize relationships between sales and advertising costs using Plotly.

- **Correlation Analysis**: Calculating the correlation between sales and advertising costs to determine the impact of TV, Radio, and Newspaper advertising.

- **Model Training**: Splitting the data into training and test sets, and training a Linear Regression model to predict future sales.

- **Prediction Function**: Implementing a function to predict sales based on user input for TV, Radio, and Newspaper advertising costs.

**3. Crypto Currency Price Prediction Model**

- **Data Import**: The notebook begins by installing yfinance and importing necessary libraries like pandas, yfinance, and datetime. It then fetches historical data for Bitcoin (BTC-USD) from a specified start date to the present day.

- **Data Preparation**: The retrieved data is organized with columns for Date, Open, High, Low, Close, Adjusted Close, and Volume. The data is also reset to ensure the index starts from 0.

- **Visualization**: A candlestick chart is created using plotly.graph_objects to visualize Bitcoin price changes over time, providing an interactive analysis tool.

- **Correlation Analysis**: The correlation between different data columns is calculated, showing a high correlation between Close, Adjusted Close, High, and Low prices.

- **Price Prediction**: The AutoTS library is used to predict future Bitcoin prices based on the historical time series data. The model explores various algorithms and configurations to forecast the next 30 days of prices.

**4. Instagram Reach Analysis and Prediction Model**

- **Data Processing**: The notebook begins with importing necessary libraries and loading the Instagram dataset. It checks for null values and provides data type information.

- **Data Analysis**: Various plots are created to analyze the distribution of Instagram impressions from different sources like Home, Hashtags, and Explore. A pie chart visualizes the proportion of impressions from these sources.
Word clouds are generated to visualize the most common words in captions and hashtags used in the posts.

- **Correlation Analysis**: The notebook examines the relationship between different factors like Likes, Comments, Shares, and Impressions to identify which factors correlate strongly with reach.

- **Prediction Model**: A PassiveAggressiveRegressor model is trained to predict Instagram post impressions based on features like Likes, Saves, Comments, Shares, Profile Visits, and Follows. The model’s accuracy is evaluated, and predictions are made using test features.

**5. Gold Price Prediction Model**

- **Importing Libraries**: The notebook begins by importing necessary Python libraries for data handling and visualization, such as yfinance, pandas, numpy, and matplotlib.

- **Data Acquisition**: It uses yfinance to download historical gold price data from 2001 to 2024, and prepares the dataset by calculating returns and lagged returns.
  
- **Model Training**: A Linear Regression model is trained using the ‘Lagged_Return’ as the independent variable and ‘Return’ as the dependent variable, based on data from 2001 to 2021.

- **Prediction & Visualization**: The model makes predictions on the test set (2022-2024), and the results are visualized in a plot showing actual vs predicted gold prices. The notebook concludes with a graph displaying the performance of the model.


**6. Spam Email Detection Classification Model**

- **Data Preparation**: The project begins by importing necessary libraries, loading the dataset from a CSV file, and performing initial data exploration. It involves checking for duplicates and missing data, resulting in a cleaned dataset of 5695 email entries.

- **Text Processing**: The next step involves downloading stopwords from NLTK and creating a function to remove stopwords and punctuation from the text. This function is applied to the ‘text’ column to clean the data.

- **Feature Extraction**: The cleaned text is then converted into a matrix of token counts using CountVectorizer, which results in a feature set with 37229 tokens.

- **Model Training and Evaluation**: A Naive Bayes Classifier is trained on the feature set and evaluated using metrics like precision, recall, and f1-score. The model shows high accuracy on both training (99.71%) and testing data (99.21%).

**7. Resume Screening Classification Model**

- **Data Preparation**: The dataset contains resumes categorized into 25 distinct job roles. The data is cleaned by removing URLs, hashtags, mentions, punctuations, and extra whitespace.
  
- **Visualization**: The distribution of resume categories is visualized using count plots and pie charts to understand the dataset better.
  
- **Text Processing**: Resumes are cleaned and tokenized, and stopwords are removed. A word cloud is generated to visualize the most common words.
  
- **Model Training**: A KNeighbors Classifier is trained using TF-IDF features. The model achieves an accuracy of 99% on both the training and test sets.

**8. SMS Spam Detection Classification Model**

- **Dataset Preparation**: The dataset is loaded and cleaned by removing unnecessary columns and renaming others. The labels are encoded for further processing.
  
- **Feature Extraction**: Text data is preprocessed using techniques like lowercasing, removing punctuation, and tokenization. The Bag of Words approach is implemented to convert text into numerical features.

- **Model Training**: The dataset is split into training and testing sets. A Multinomial Naive Bayes model is trained on the training data.

- **Model Evaluation**: The model’s performance is evaluated using metrics like accuracy, precision, recall, and F1 score, achieving high accuracy and precision.

**9. Hate Speech Detection Model**

- **Data Preparation**: The code imports necessary libraries and reads training and test datasets for hate speech detection.

- **Text Cleaning**: It preprocesses text data by converting to lowercase and removing unwanted characters like mentions, URLs, and non-alphanumeric characters.

- **Handling Imbalance**: The training data is balanced by upsampling the minority class to match the majority class.

- **Model Training**: A pipeline using CountVectorizer, TfidfTransformer, and SGDClassifier is created and trained on the processed data, achieving an F1 score of 0.969.
