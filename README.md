# AppliedDataScienceCapstoneIBM
This is the creation of the Capstone Project Notebook for IBM's Applied Data Science Capstone.


# Problem Introduction
Imagine the year is 2020 and you are living in the densely populated city of Columbus, Ohio in the midst of the COVID-19 pandemic, and you are starting to feel intense sickening pain. This alarms you, you want to find a place to get tested for a virus. However, testing may be in short supply and you are not sure where to go. The problem I am trying to solve is where testing locations should be set up in order to best test people from the COVID-19 pandemic. 

3 sets of data are: 
- four-square api data
- zip code and demographic data
- Covid-19 Cases by ZIP for Ohio 

As well as current testing locations.
 
This will be used to solve the problem, by first understanding:
- What factors are likely to cause COVID-19
- Where should testing locations be placed, in order to accommodate everyone to a fair and equal extent.
- With the four-square api I will get hospital and pharmacy locations, the reason for this is because it is reasonable for people to seek medical care from either location, and as a result people would go there.

The major variables are:
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
