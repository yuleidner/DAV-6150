# DAV-6150
 Data Sceince Class Fall 2021

 M2: Cross Validating a Linear Regression Model

 		This notebook explores data from the UC Irvine machine learning archive to gain some familiarity with the dataset, and get a general sense of what features are available. Then, it constructs a pair of cross-validated linear regression models that predict the weight of a vehicle. The cross-validated performance of the two models is then compared to identify the preferred model, and concluding thoughts added.

		The EDA was poorly done, but has a good example of machine learning with R^2 metrics derived from the K-fold cross validation of a linear regression model

M3: Cleaning a Messy Data Set

	This notebook will explore and clean a dataset of wine attributes that suffers from a variety of data integrity and usability issues. Our main goal is to prepare the individual variables for modeling; therefore we will attempt to Normalize and Standardize Continous features where appropriate. We will also create Dummy Variables for Ordinal Categorical features. We will start by exploring the distributions of the individual variables, bringing in what domain expertise we can learn without access to a subject matter expert. We will then prepare the features according to our findings, while examining our changes to ensure they are appropriate.

		includes code for 
			a combined histogram and boxplot
			Multiple Null Imputes

		Lessons Learned
			Finish early enough to check spelling and grammar
			As part of your EDA work you should develop some domain knowledge so that you are more informed regarding the possible data values 
			It is not appropriate to include categorical data within a pearson's correlation matrix since categorical data is not quantitative
			analysis performed to locate missing data values should be part of your EDA work, not your data preparation work
			understanding of Box-Cox methods is clearly amiss.
				Within your data preparation work you apply a log transform, a square root transform, and then subsequently apply the Box-Cox method. Box-Cox already INCLUDES the application of both a log transform and a square root transform
			LabelAppeal is clearly an ORDINAL categorical variables. As such, if we convert it to binary dummy variables we will not retain the ordinal information contained within the original ordinal data. Therefore, you should rethink your data prep approach for that variable. It is NEVER appropriate to convert ordinal categorical data to binary dummy variables. Please refer to the Module 3 Assigned Readings for more information on this.

M4: Feature Selection & Dimensionality Reduction

	This dataset was published by mashable which is an entertainment platform. It contains information such as how many words are in the title, how many unique words in the content, which day the article was published, and title polarity. One can utilize the information presented in the dataset to predict when the good time is to publish an article, or how many words that are in the title would be a good estimator to predict the number of shares for an article.

	Research Question: How can we predict the number of times an online news article will be shared? To answer this question, we need to perform exploratory data analysis (EDA) on our dataset and evaluate how our variables relate to the number of shares. We will transform the data to better prepare it for predictive models, fixing any problem areas we identify in our EDA. Next we will perform feature analysis and principle component analysis to reduce our feature set to something that is accurate but without unneeded complexity. Finally, we will analyze this model and compare it to other possible models to assess its effectiveness.

		Your approach to EDA + feature selection / dimensionality reduction + model development is very much on target.
		 In your initial analysis of the data set, you appear to be relying upon the output of the .info() function to specify the data types of the attributes. This approach is not valid since the output of that function is in no way indicative of the data types of the actual variables.
		 applying PCA and interpreting its output. For your feature selection work, use of RFECV is OK, but it would be to your benefit to gain some experience with additional methods, e.g., forward selection, use of variance thresholds, etc.
		 Regression Model Evaluation
		 Good job of trying a variety of models based on different treatments of the data.

M5: Classification Model Performance Metrics
	
	customized functions produce results that are validated by the scikit-learn pre-built functions including explanations as to why the results of your custom built functions vary slightly from those of the pre-built scikit-learn functions.

M6: Project 1



