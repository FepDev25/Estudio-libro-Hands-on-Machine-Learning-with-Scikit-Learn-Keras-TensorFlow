# End-to-End Machine Learning Project

## Get the data

- Jupyter Notebook to download and load the housing data:
  - [Download the data](code/fetch_load_data.ipynb)

## Take a Quick Look at the Data Structure

- Looking at the first few rows of the dataset:
  - ![First few rows](img/7.png)
  - Each row represents one district.
  - There are 10 attributes: longitude, latitude, housing_median_age, total_rooms, total_bedrooms, population, households, median_income, median_house_value, and ocean_proximity.
- Description of the dataset:
  - ![Dataset description](img/8.png)
  - There are 20,640 instances in the dataset.
  - total_bedrooms attribute has only 20,433 non-null values, meaning that 207 districts are missing this feature (take care of this later).
  - All attributes are numerical, except for ocean_proximity (text and categorical). Find out how many categories exist:
    - ![ocean_proximity value counts](img/9.png)
- The describe() method shows a summary of the numerical attributes:
  - ![Numerical attributes summary](img/10.png)
  - The count, mean, min, and max rows are self-explanatory.
  - Null values are ignored.
  - The std row shows the standard deviation.
  - The 25%, 50%, and 75% rows show the corresponding percentiles (the median is the 50th percentile).
- Histogram: shows the number of instances (on the vertical axis) that have a given value range (on the horizontal axis).
  - ![Histograms of all attributes](img/11.png)
