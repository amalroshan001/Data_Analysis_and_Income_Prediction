- Open Jupyter Notebook ;  
- Imported Neccessory Libraries for after uses ;
- Imported Libraries :
  • Pandas
  • Numpy
  • matplotlib.pyplot
  • seaborn
  • from sklearn import preprocessing
  • from imblearn.over_sampling import SMOTE
  • from sklearn.model_selection import train_test_split
  • from sklearn.linear_model import LogisticRegression
 
- Read the Income Datasets using pandas library; 
- Checked Basic Information about the dataset (shape,info,columns,dtypes,null values,describe);  
- Renamed a column named 'nan' to 'Age' by using rename function ; 
- To Check for any missing values or any symbols printed unique of every Features by using a for loop ;
- There was symbol like '?' in this dataset so we replaced it with null values ;
- Took a sum of null values and visualised null values using heatmap in seaborn library ;
- Then Filled the null values by using ffill (Forward Fill - It replaces the NULL values with the value from the previous row (or previous column, if the axis parameter is set to 'columns' ) )
- Then Checked for duplicated values and found 24 dupicates and dropped those duplicates because it was a small amount of data;

- Then Started to visualise all the features one by one;
- first plotted data using hist
- Then classified data into two those who have greater than 50k into a variable and those who doesn't have into another ;
- Then plotted both of the data with a feature named 'workclass' using countplot ;
- Then used catplot and plotted box then found average income with age and also found some outliers ;
- After all the cleaning is done then saved the cleaned dataset into a new csv file;

- Started the Encoding
- First used LabelEncoder instance,( fits it to the provided categories, and then transforms the categories into integers in one line.)
- The datas were imbalanced and to balance the data we used SMOTE technique to create synthetic values ;
- Then Splitted the data for testing and training using train_test_split ;
- Then started to create a model using LogisticRegression ;
- Then predicted the values that have tested and checked accuracy,score,confusion_matrix and so on...;

- Open the cleaned excel file we worked in PowerBi
- Stacked Column Chart - Sum of Capital Gain by Sex
- Pie Chart - Sum of Capital Gain by Education
- Donut Chart - Sum of Capital Gain by Marital-Status
- Funnel Chart - Sum of Capital by Workclass
- Matrix - Rows : workclass , marital-status
         - Columns : Sex
         - Values : Sum of Capital Gain
- Cards :  Sum of Capital Gain , Sum of Capital Loss , Count of Income
- Slicer - Income

