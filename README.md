# matplotlib-challenge

This jupyter notebook examines mice in a study. The following datapoints are given for each mouse:
   Mouse ID
   Drug Regimen
   Sex
   Age_months
   Weight (g)
   Timepoint
   Tumor Volume (mm3)
   Metastatic Sites

The following visual methods were used to present the data:
   Bar plot for the Total Number of Measurements for each Drug Regimen.
   Pie chart for the distribution of male vs female mice.
   Boxplot of Tumor Volume (mm3) at Latest Timepoint for 4 Drug Regimens
   A line plot to track the tumor volume over time for a random mouse from the Capomulin regimen.
   A scatter plot with linear regression to evaluate the relationship between Average Tumor Volume vs. Mouse Weight for the Capomulin Regimen.

Opportunities arose to try several different methods to ensure the same result (using dictionary comprehension, .pivot, etc. to provide the dataframe for Boxplot, for example). These were labeled as such in an attempt to reduce confusion.

Limitations:
The data was analyzed for opportunities to clean and reduce error. 
We identified a mouse that had data from duplicate timepoints. However, the data at these duplicated timepoints was different, making it difficult to decide what data for this mouse (g989) to keep.
Additionally, not all mice have the same number of timepoints data. Instructions to analyze the "last timepoint" for each mouse are consequently ambiguous and may not be sufficiently considered.

##Observations
#1. The study mice are fairly evenly distributed across gender.
#2. Mice treated with Capomulin and Ramicane has smaller tumor volume measurements are their last timepoint than those treated with Ceftamin or Infubinol based on the box plot.
#3. For mice on the Capomulin regimen, weight is strongly positively correlated with tumor volume (ie  mice with lower weights are more likely to have lower tumor volumes;   mice with higher weights are more likely to have higher tumor volumes).