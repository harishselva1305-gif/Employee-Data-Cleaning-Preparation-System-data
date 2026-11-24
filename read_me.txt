Sample dataset
Enter the following data in the Raw_Data worksheet.
Emp_ID	Employee_Name	Department	Location	Join_Date	Salary	Status
EMP1001	Rahul Kumar	IT	Chennai	15-01-2022	35000	Active
EMP1002	Priya Sharma	HR	Bangalore	20-03-2021	42000	Active
EMP1003	Arun Kumar	Sales	Chennai	10-06-2023	28000	Active
EMP1004	Divya Raj	Finance	Hyderabad	05-08-2020	50000	Active
EMP1005	Karthik S	IT	Bangalore	12-12-2022	38000	Inactive
EMP1006	Sneha Devi	HR	Chennai	18-04-2024	30000	Active
EMP1007	Rahul Kumar	IT	Chennai	15-01-2022	35000	Active
EMP1008	Naveen Kumar	Sales	Hyderabad	25-09-2021	45000	Active

Note: EMP1007 is intentionally duplicated so you can practise removing duplicates.


Task 1: Workbooks, worksheets, cells and ranges
- Create a workbook named Employee_Data_Analytics.xlsx.
- Create the four worksheets listed above.
- Enter the dataset starting from cell A1.
- Select the range A1:G9.


Task 2: Entering and formatting data
Apply these formatting rules:
- Heading: Bold with background colour.
- Employee ID: Text format.
- Joining Date: DD-MM-YYYY.
- Salary: Currency format (₹).
- Adjust column widths.
- Apply borders to the dataset.


Task 3: Sorting and filtering
Practise the following:
1. Sort employees by salary from highest to lowest.
2. Sort employees alphabetically by name.
3. Filter only IT department employees.
4. Filter employees whose status is Active.
5. Filter employees located in Chennai.


Task 4: Removing duplicates
1. Select the employee dataset.
2. Navigate to Data → Remove Duplicates.
3. Select all columns to identify completely duplicated records.
4. Click OK.
Expected result: 7 unique employee records.


Task 5: Text functions
Assume Employee ID is in A2 and Employee Name is in B2.
Function	Excel formula	Purpose
LEFT	=LEFT(A2,3)	Extract EMP
RIGHT	=RIGHT(A2,4)	Extract employee number
MID	=MID(A2,4,4)	Extract middle characters
TRIM	=TRIM(B2)	Remove extra spaces

For example:
Text function output
Original ID	EMP1001
LEFT	EMP
RIGHT	1001
MID	1001


Task 6: Date functions
Assume Join_Date is in E2.
Function	Formula	Purpose
TODAY	=TODAY()	Current date
YEAR	=YEAR(E2)	Extract joining year
MONTH	=MONTH(E2)	Extract joining month
DATEDIF	=DATEDIF(E2,TODAY(),"Y")	Calculate completed service years

Additional formula:

=DATEDIF(E2,TODAY(),"YM")

This calculates the remaining months after completed years.


Task 7: Conditional formatting
Apply conditional formatting to the Salary column.
- Salary greater than ₹40,000 → Green.
- Salary between ₹30,000 and ₹40,000 → Yellow.
- Salary below ₹30,000 → Red.
Also highlight duplicate Employee IDs using:

Home → Conditional Formatting → Highlight Cells Rules → Duplicate Values.


Task 8: Data validation and drop-down lists
In the Lists worksheet, create:
Department	Location	Status
IT	Chennai	Active
HR	Bangalore	Inactive
Sales	Hyderabad	
Finance	Mumbai	

Create drop-down lists:
1. Select the Department cells in Clean_Data.
2. Go to Data → Data Validation.
3. Select Allow → List.
4. Enter the department list as the source.
5. Repeat for Location and Status.
Now users can select values instead of typing them manually.