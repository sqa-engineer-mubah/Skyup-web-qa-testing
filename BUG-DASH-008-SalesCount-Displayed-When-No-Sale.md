# Bug ID: UI-001  

## Title  
Sales Count Displays Incorrect Value When No Sale is Recorded  

## Environment  
- Application: SkyUp Web  
- Module: Dashboard  
- Browser: ( Chrome)  

## Description  
The "Sales Count" column in the Dashboard table is displaying incorrect values. In scenarios where the "Sold" status is marked as false (✖), the Sales Count still shows a value of 1. This results in a mismatch between the sales status and the derived sales count.
 

## Steps to Reproduce  
1. Navigate to the Dashboard  
2. Locate the data table displaying sales records  
3. Identify a row where the "Sold" column shows  (no sale)  
4. Observe the corresponding "Sales Count" value  

## Actual Result  
- "Sold" status is  (No Sale)  
- "Sales Count" is displayed as 1  

## Expected Result  
- If Sold =  Sales Count should be 0  
- If Sold =  Sales Count should be 1  
- Sales Count must always be consistent with Sold status  

## Impact  
- Leads to incorrect sales reporting  
- Misrepresents sales performance metrics  
- Affects business decisions and reporting accuracy  

## Severity  
High (Data Integrity Issue)  

## Priority  
High  
