
# Phishing Website Detection


For an easy execution of the different parts of the project, we chose to split the code into 4 different and independant notebooks forming the project pipeline:

**Part1:**
Part1_Web_Scraping-and-data-collection: This jupyter notebook collects the data from webpages using webscraping techniques and from an external dataset (kaggle reference). It requires to have an adopted version of chromedriver of your navigator with a correct path.

Output => phish_website.csv & legitimate_websites.csv

PS: The execution of this notebook may take a lot of time, you can find the result files in the Datasets Folder.

**Part2:**

Part2_features_extraction: This notebook iterates through the resulting list of links and generate the required feature.

Output: ligit_file.csv & phish_file.csv

PS: The execution of this notebook took a lot of time, we had to divide the task and generate 6 different files. Also, it may require external packages as whois and threading.

You can also find the result files directly in the Datasets Folder.

**Part3:**

Part3_Data_construction_and_cleaning: This notebook does the merging and union of the resulting files of the previous task and does the cleaning and visualisation tasks to generate the final dataset for the models.

Output: database_websites.csv (exists in the Datasets Folder)


**Part4:**

Part4_Websites_Classification: This notebook uses the previous dataset to train and optimize different models in order to fulfill the project objective: Websites Classification into legitimate and phishing categories.
