# Datasheet Template

As far as you can, complete the model datasheet. If you have got the data from the internet, you may not have all the information you need, but make sure you include all the information you do have. 



## Motivation

- For what purpose was the dataset created? 
- Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?

i) Purpose of Dataset: The dataset was created to analyze and predict exchange rate stability in Nigeria based on economic indicators by scrapping and selecting economic variables from the Website of the World Bank. 

ii) Creator and Entity: The entire dataset was curated by the World Bank. 

 
## Composition

- What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)? 
- How many instances of each type are there? 
- Is there any missing data?
- Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by    doctor–patient confidentiality, data that includes the content of individuals’ non-public communications)?

i) Instance Representation: The instances in the dataset represent economic indicators related to exchange rate stability, real interest rate, and foreign reserves in Nigeria.

ii) Number of Instances: The dataset comprises 132 entries.

iii) Missing Data: The dataset contains some missing values in certain indicators, which were handled during preprocessing.

iv) Confidential Data: The dataset does not contain data that is considered confidential or protected by legal privilege. The dataset is largely publicly available. 


## Collection process

- How was the data acquired? 
- If the data is a sample of a larger subset, what was the sampling strategy? 
- Over what time frame was the data collected?

i) Data Acquisition: The data was acquired by scraping economic indicator data from the website of the World Bank.

ii) Sampling Strategy: The dataset represents a sample of the available economic indicators for Nigeria over the time frame from 2000 to 2021. The whole dataset from the World Bank starts in 1960 and covers many more socio-economic indicators. 

iii) Collection Time Frame: The data was collected over the span of several years, from 2000 to 2021. The whole dataset from the World Bank starts in 1960 and covers many more socio-economic indicators. 

## Preprocessing/cleaning/labelling

- Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section. 
- Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)? 

i) Preprocessing: The data underwent preprocessing to handle missing values, scale the features, and split it into training, validation, and test sets.

ii) Saving Raw Data: Both the raw data scrapped from the World Bank's website and the preprocessed dataset were saved for reference and potential future use in the code. A wider data dictionnary is available on the World Bank's website.
 
## Uses

- What other tasks could the dataset be used for? 
- Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms? 
- Are there tasks for which the dataset should not be used? If so, please provide a description.

i) Other Possible Tasks: The dataset could potentially be used for analyzing trends in the Nigerian economy, conducting scenario analyses, and exploring relationships between economic indicators.

ii) Impact Considerations: The composition and collection process of the dataset are designed to provide accurate exchange rate stability predictions. However, users should be aware that the accuracy of predictions is influenced by data quality, and should exercise caution when making critical decisions based on the model's output.

iii) Restricted Uses: The dataset should not be used for making high-stakes financial decisions without considering additional expert advice.

## Distribution

- How has the dataset already been distributed? 
- Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?  

i) Previous Distribution: The dataset has not been previously distributed and is currently for academic research purposes.

ii) IP and ToU: Whilst the dataset is widely avaible, it is subject to copyright (as reference must be made to originator of the dataset namely the World Bank) and applicable ToU as described in this link: https://data.worldbank.org/summary-terms-of-use . 


## Maintenance

- Who maintains the dataset?

The expanded dataset and socio-economic indicators are maintained by the World Bank. 

