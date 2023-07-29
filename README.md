# Student-Performance_Python-Data-Analysis
An analysis of the correlation between traits of a student and their resulting test score. Traits in this data set are ethnicity (grouped, not explicitly defined), gender, parental level of education, lunch time, and completion of a test preparation course which are compared to their resulting scores in math, reading, and writing.
OVERVIEW
After introducing the dataset and defining the objective, a doctscipt is created to outline all relevant information of the dataframe
EXPLORATION
Seaborn is used to create visualizations of the student population per respective TRAIT column (Gender, Ethnicity, Parental Education, Lunch, and Test Prep)
PROCESSING
A distribution plotting code is developed and utilized with the Seaborn pairplot function, defined as dist_plot(), to graph the correlation between each TRAIT column and the 3 standardized testing scores.
The distribution plot is a unique type of graph and difficult to interpret, but it should be mainly noted that the diagonal plots provide the most coherent visualization of correlation
an ANOVA function is developed as a supplement to the dist_plot() to provide a numerical correlation value. The ANOVA function helps in the sense that it defines whether or not a correlation exists at all to ease further analysis.
INSIGHTS
This is where the findings are addressed and we look back to identify any outliers and possible faults. Here we identify that parental education is an outlier that doesnt particularly partain to the student themselves. 
To further explore this, we want to find whether or not parental education has any effect on the student. This step can be solved with a simple line of code, in which I calculate the percentage of "high-scoring students" which we define as above a 70. 
From this we find that higher parental education leads to a higher percentage of high scoring students, thus a correlation definitely exists in this variable. 
CONCLUSION
From our findings in this analysis, we can conclude that every factor represented in this dataset has an effect on the outcome of a student's performance on their standardized tests
