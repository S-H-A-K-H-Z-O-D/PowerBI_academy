# Lesson 12
**Topic:** Text, Informational and Logical Functions  
**Prerequisites:** Connect SQL Server to Power BI desktop and import DimCustomer table from AdventureWorksDW database (2019)  
**Questions:**

### Basic Level (1–10)
- Concatenate First and Last Name  
- Convert Email Address to Uppercase  
- Extract First 3 Characters from First Name  
- Count Characters in Last Name  
- Convert First Name to Lowercase  
- Trim Spaces in EnglishEducation  
- Repeat '\*' Character Equal to Length of First Name  
- Get Last 4 Characters of Phone Number  
- Format YearlyIncome to Currency with 2 Decimals  
- Check If FirstName and LastName Are Exactly the Same  

### Intermediate Level (11–20)
- Find If 'Manager' Appears in Occupation (Case Sensitive)  
- Search for 'graduate' in EnglishEducation (Case Insensitive)  
- Extract Characters 3–7 from First Name  
- Replace Area Code in Phone Number with 'XXX'  
- Format BirthDate as 'DD-MM-YYYY'  
- Create Initial + Last Name Format (e.g. J.Smith)  
- Capitalize First Letter of FirstName, Lowercase the Rest  
- Substitute Dashes with Spaces in Phone  
- Convert BirthDate Year to Numeric Using VALUE  
- Show YearlyIncome Rounded to 1 Decimal Without Commas  

### Advanced Level (21–30)
- Customer Code: First 2 Letters of LastName + Last 2 of CustomerKey  
- Validate Email Ends with '.com' and Contains '@'  
- Extract Domain Name from EmailAddress  
- Mask Phone Number Except Last 4 Digits  
- Proper Casing of Last Name (simulate manually)  
- Replace Multiple Spaces in EnglishOccupation with Single Space  
- Generate Custom ID: Initials + Birth Year (e.g., JD\_1985)  
- Remove Hyphens and Convert Phone to Number  
- Create a measure or calculated column that categorizes customers into segments using both ```EnglishEducation``` and ```YearlyIncome```.  
  If the education is "Graduate Degree" and income > 90000 → "Elite"  
  If education is "Bachelors" and income between 60000–90000 → "Professional"  
  If education is "High School" → "Basic"  
  Otherwise → "Other"  
- Create a measure that returns:  
  Total Customers if no selection  
  Customer count for selected Gender  
  If more than one gender is selected, return "Multiple Values Selected"  

