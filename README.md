
####
ALL THE OTHER STEPS ARE WELL INDICATED IN THE NOTEBOOK FILE ATTACHED  CHURN EDA AND REGRESSION ANALYSIS
****For any Explorer, **
SWITCH TO CODE VIEW TO HAVE  A BETTER LOOK  code view  is indicated as < >
#######

# ML-EDA
Perfoming EDA on a dataset
Steps undertaken and the Findings
#Step 1-Getting the dataset to jupyter workbook
  Command-data=pd.read_csv(r"C:\Users\USER\Desktop\insurance.csv")
#Step 2. Viewin the dat
  command:data.head()-Got the first 5 Rows.
#3Getting some info about the dataset
    Found no-null values
 #4.Checking for duplicate
  commande-data.duplicate().sum() --Found 0
  
  
  
###################
Perfoming linear Regression
#######################
Step 1 Importing  class LinearRegression from sklearn.linear_model:
   Command:from sklearn.linear_model import LinearRegression
Step2 :Loading the data to work with
  Assigning X and Y
  Command=X=data["age"] , y=data["charges"]
Step3: Reshaping the data
     Command: x_matrix=x.values.reshape(-1,1)
             x_matrix.shape
             
Step4: creating  a linear regression model and fit it using the existing data.
    model = LinearRegression()
    model.fit(x, y)
    model = LinearRegression().fit(x, y)
  Step5:The result of the fitted Model
  .....
      Command:
      Score = model.score(x, y)
      print(f"coefficient of determination: {Score}")
    
    
             
 

   

