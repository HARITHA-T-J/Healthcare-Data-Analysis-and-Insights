# Healthcare-Data-Analysis-and-Insights
DATA CLEANING:-
1) Check for the number of missing values marked with '?' in each column of the “Medical Examinations” Table and "Hospitalization Details" Table-Using filter we can check the number of ?in each coloumn 
2) Fill in the missing values of ‘month’ with Sep and ‘year’ with its average rounded to the nearest integer- ? replaced by the month Sep using format function data trim and capitalize each word.
3) Determine the most frequently occurring values in the ‘smoker’, 'Hospital tier' and 'City tier' columns, and fill in the missing values accordingly - using count if function checked the most frequent occured values in hispital tier column,smoker and city tier column and replaced ? using most frequent occured value.Using format function data trim,capitalize each word.
4) If any 'State ID' values are missing, consider filling them with 'Unknown' or using another appropriate strategy-using Replace function ? are replaced by missing values,Using format function trim,Capitalize each word and clean.
5) DATA TRANSFORMATION:-
 1) Split the ‘names’ column in the “Customer Names” Table into 3 meaningful columns:‘Title’, ‘First Name’, and ‘Last Name’-Removed top row and split -using split function created three columns split by delimiter and title column split by number of characters from left and remaining titled as first name.
2)Convert the "NumberOfMajorSurgeries" column in the “Medical Examinations” Table to numerical data by replacing non-numeric characters with meaningful numerical values- Using replace function non neumeric value " No major surgery " to zero.
3) Check for inconsistencies in the 'Heart Issues' and 'smoker' columns and propose corrective actions if necessary-Using  format function capitalize each word ,trim,clean.smoker column already cleaned,trimed and capitalize each word.
4) Create a new column named “Weight Status” that categorizes BMI into different categories as below- Add a new colun named Weight Status using this syntax if [BMI] < 18.5 then "Underweight"else if [BMI] < 25 then "Normal Weight"else if [BMI] < 30 then "Overweight"else "Obesity"
5) Create a new column named “Diabetes Status” and fill it as per the information givenbelow:Add a column named Diabetes Status used this syntax if [HbA1C] = null then nullelse if < 5.7 then "Normal"else if < 6.5 then "Prediabetes"else "Diabetes"
6) Merge ‘year’, ‘month’ and ‘date’ columns in the “Hospitalization Details” Table into one column named ‘Date of Birth’ and format it in ‘DD-MMM-YYYY’ custom format -Using concat function add three columns into one column.=CONCAT([@date],"-",[@month],"-",[@year]) and using Text function =TEXT([@[Date of Birth]],"dd-mm-yy").
7)  Calculate the ‘Age’ of each customer based on their ‘Date of Birth’ and the date ofcollection of the dataset, which is 8th June 2023.Using =DATEDIF([@[Date of Birth2]],DATE(2023,6,8),"y")
8) Format ‘charges’ column as currency ($).charges column formated by currency symbol (ribbon-excel)
9) Data Exploration, Analysis & Visualization:
10) 
