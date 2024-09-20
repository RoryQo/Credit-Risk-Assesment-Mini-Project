# Credit-Risk-Mini-Project

#### Results
This project creates a model to predict a person's credit risk, high approximated as bad credit or low approximated by good credit. Using a logistic regression model, we could predict credit risk 80% with the testing data correctly. While not the most accurate model, it is a quick and simple model, using readily available information from a client, because of this, the model would be best implemented as a litmus test for bank branches when sorting customers into high-risk groups for financial services, saving bank and client time when discussing potential client services, before a time intensive credit report is pulled.   


#### Description of Data
Each entry represents a person who takes a credit by a bank. Each person is classified as a good or bad credit risk according to the set of attributes
##### Features
1. `Age` (numeric)
2. `Sex` (text): male, female
3. `Job` (numeric): 0 - unskilled and non-resident, 1 - unskilled and resident, 2 - skilled,  3 - highly skilled)
4. `Housing` (text): own, rent, or free
5. `Saving` (text): little, moderate, quite rich, rich
6. `Checking` (text): little, moderate, rich
7. `Credit_amount` (numeric, in DM)
8. `Duration` (of the debt)(numeric, in month)
9. `Purpose` (of the debt) (text): car, furniture/equipment, radio/TV, domestic appliances, repairs, education, business, vacation/others
10. `credit_history`: 
   * 0 : delay in paying off in the past       
   * 1 : critical account/other credits elsewhere
   * 2 : no credits taken/all credits paid back duly
   * 3 : existing credits paid back duly till now
   * 4 : all credits at this bank paid back dul
11. `installment_rate`: Installment rate in percentage of disposable income. 
1 -'35 or more', 2 - '25 to 35', 3 - '20 to 25', 4 - 'less than 20'
12. `other_debtors`: Other debtors/guarantors. 1 - 'none', 2 - 'co-applicant', 3 - 'guarantor'
13. `number_credit`: Number of existing credits at this bank. 1 - '1', 2 - '2-3', 3 - '4-5', 4 - '6 or more'
14. `telephone`: 1 - 'no', 2 - 'yes (under customer name)'
15. `people_liable`: Number of people being liable to provide maintenance for. 1 - '3 or more', 2 - '0 to 2'
16. `foreign_worker`: 1 - 'yes', 2 - 'no'

##### Target
`Credit_risk` (binary): 0 - bad, 1 - good
