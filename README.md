# AppliedDataScienceCapstoneIBM
This is the creation of the Capstone Project Notebook for IBM's Applied Data Science Capstone.


# Problem Introduction
Imagine the year is 2020 and you are living in the densely populated city of Columbus, Ohio in the midst of the COVID-19 pandemic, and you are starting to feel intense sickening pain. This alarms you, you want to find a place to get tested for a virus. However, testing may be in short supply and you are not sure where to go. The problem I am trying to solve is where testing locations should be set up in order to best test people from the COVID-19 pandemic. 

3 sets of data are and (what they are backed up as are): 
- four-square api data (HospitalAndPharmacy.csv)
- zip code and demographic data (ZipInformation.csv)
- Covid-19 Cases by ZIP for Ohio (ZipCases.csv)

As well as current testing locations.
 
This will be used to solve the problem, by first understanding:
- What factors are likely to cause COVID-19
- Where should testing locations be placed, in order to accommodate everyone to a fair and equal extent.
- With the four-square api I will get hospital and pharmacy locations, the reason for this is because it is reasonable for people to seek medical care from either location, and as a result people would go there.

The major variables and functions are:
- Data Frames: 
	- zip_info_df: Gets demographics by ZIP
	- hp_df: Hospital and Pharmacy Location Information
	- zip_cases_df: Covid-19 cases by zip.
	- grand_zip_df: zip_info_df and zip_cases_df combined
	- lat_long_df: latitude and longitude of grand_zip_df
- Arrays & Lists:
	- testingLocations: Has current Testing Locations
	- corr_arr: correlation grand_zip_df has with Cummulative Cases
	- INDEXARRAY: Correlation indices of all relevant variables
	- corr_arr_spearman: Spearman correlation with grand_zip_df and Cummulative Cases
	- INDEXARRAYSPEARMAN: Top correlated variables from corr_arr_spearman
- Functions:
	- kmeansweight: Gives the kMeans clustering a weighting	
	- zip_info: webscrapes demographic data
	- custom_metric: Custom Metric used for dendrograms
	- custom_metric0: Custom Metric used for dendrograms Spearman
	
# There is a special section to load csv files called CSV backup and loading section. There is a stop cell with contents "print(df" to stop running contents.

Parts with their description are:
- Part 1 Data Retrieval: Involves gathering of data with webscraping
- Part 2 Modifying of Data: Modified column names to allow for proper reading
- Part 3 Filtering and Adjusting of Data: Filtering data.
- Part 4 Data Exploration: Exploring the data to better understand what is going on
- Part 5 Clustering and Association Algorithms: Run clustering algorithms and create new models
- Part 6 Results via Maps: Shows results created on maps  

