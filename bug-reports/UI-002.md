# Bug ID: UI-002  

## Title  
Sales Credit (0.5) Assigned in Turn Case Even When No Sale Occurred  
  

## Environment  
- Application: SkyUp Web  
- Module: Dashboard  
- Browser: (Chrome)    

## Description  
In cases where a deal involves two sales representatives (Turn scenario), the system assigns 0.5 sales credit to each rep. However, this credit is being assigned even when no sale has occurred which is incorrect.

## Preconditions  
- A record exists with two sales reps (Turn case)  
- Sold status is  (No Sale)  

## Steps to Reproduce  
1. Navigate to Dashboard  
2. Locate a record with two sales reps (Turn case)  
3. Ensure Sold = No Sold 
4. Observe sales credit/count for both reps  

## Actual Result  
- Each sales rep receives 0.5 credit  
- Even when Sold = No Sold

## Expected Result  
- If Sold = Yes  Each rep gets 0.5 (valid)  
- If Sold = No  Each rep should get 0 credit  

## Impact  
- Incorrect sales performance tracking  
- Inflated sales metrics  
- Affects commission and reporting accuracy  

## Severity  
High (Business Logic Issue)  

## Priority  
High  
