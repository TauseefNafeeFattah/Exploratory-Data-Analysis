# Exploratory-Data-Analysis
This is a data science project where K-Means Clustering algorithm is used to find the best accommodation of student around University of Toronto. The accommodation has been classified for students based on their preferences on amenities, budget and proximity to the location.
## Workflow
![workFlow](https://user-images.githubusercontent.com/57330415/211214752-1e32d173-bd1a-4e35-aff5-b5e778f9d5d5.png)
1. **Collect Data**: Utilized [Food Choices](https://www.kaggle.com/datasets/borapajo/food-choices) dataset from kaggle to differentiate between students.
2. **Clean data and Visualize using Boxplot**: Utilized pandas dataframe to choose suitable parameters and cleaned the data appropriately. Used seaborn library to create boxplots to visualize the data.
3. **Run K-Means Clustering**: Ran K-Means clustering on cleaned data for arbitrary values of K. For K=3 a clear demarcation on the basis of income was seen. High income students pay more on meal out, eat less fruites, mostly stay on campus, excercise more and cook less, while Low income student does the opposite in these cases.
4. **Get Geolocational Data from HERE API**: Used HERE API to get the real time geolocation data around University of Toronto. Useful parameters were selected and the data was cleaned.
5. **Cluster Geolocational Data**: Clustered the recieved data using K=3.
6. **Plot the Locations on Map**: Used Folium to plot the clustered data on a Map.
## Implementation Results:
![UofTMapOutput](https://user-images.githubusercontent.com/57330415/211214759-5c3d1fa2-5208-461a-9b95-bde4cb4b53eb.png)
## Observation:
1. Cluster 0(Green) has maximum department stores, cafe and gyms.  
2. Cluster 1(Yellow) has minimum department stores, cafe and gyms.  
3. Cluster 2(Red) has more gyms but less department stores, and cafe.  
