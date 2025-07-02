# CASE STUDY : PALMORA GROUP HR ANALYSIS 
The Palmoria Group, a manufacturing company based in Nigeria, is embroiled in issues bordering on gender inequality in its 3 regions. Unfortunately, the media recently published the news with the headline “Palmoria, the Manufacturing Patriarchy”. This doesn’t look good for the owners of the business, based on their ambition to scale the business to other regions and even overseas. Cases like this can only spiral downwards, revealing other issues like the gender pay gap, amongst other possible issues. The CEO of Palmoria, Mr Ayodeji Chukwuma, is keen to address these issues before they get out of hand. The CHRO, Mr Yunus Shofoluwe, has been assigned the task to identify key areas within the business that could give rise to issues and address them immediately. Mr Shofoluwe decided to recruit you as an HR Analytics expert to analyse the company’s HR data and come up with recommendations for management’s attention. “Now, the future of gender equality in Palmoria lies in your hands” – the exact words of Mr Shofoluwe before he handed the data to you.

## CASE SCENARIO 
•	Analyse the company data and generate insights that the Palmoria management team would need to address 

•	Your analysis should be visualised using appropriate charts 

•	Your focus should be on gender-related issues within the organization and its regions 

•	The insights required are based on your discretion. However, Mr Gamma, as an insider, has offered to give you pointers on areas you need to pay attention to.

## Required: 
•	Generally, there are two genders in the organization. However, some employees refused to disclose their gender. You would need to assign a generic gender status to these employees 

•	Some employees are without a salary because they are no longer with the company. You will need to take those employees out 

•	Lastly, some departments are indicated as “NULL”. These departments would also need to be taken out.

## Pointers from Mr Gamma 
1.	What is the gender distribution in the organization? Distil to regions and departments 

2.	Show insights on ratings based on gender 

3.	Analyse the company’s salary structure. Identify if there is a gender pay gap. If there is, identify the department and regions that should be the focus of management 

4.	A recent regulation was adopted which requires manufacturing companies to pay employees a minimum of $90,000

       •	Does Palmoria meet this requirement? 

       •	Show the pay distribution of employees grouped by a band of $10,000. For example: 

       •	How many employees fall into a band of $10,000 – $20,000, $20,000 – $30,000, etc.? 

       •	Also visualize this by regions

## Case Questions 
5.	Mr Gamma thought to himself that since you were already working on the employee data, you could help out with allocating the annual bonus pay to employees based on the performance rating. He handed you another data set that contains rules for making bonus payments and asked you to: 

       •	Calculate the amount to be paid as a bonus to individual employees 

       •	Calculate the total amount to be paid to individual employees (salary inclusive of bonus) 

       •	Total amount to be paid out per region and company-wide

## Data Source
The data for this Analysis was gotten from Digital SkillUp Africa (DSA) Learning Management System (LMS) as part of my final project.

## Tools Used for the Analysis
The tool for this is Power BI. You can download it via this link (https://www.microsoft.com/en-us/download/details.aspx?id=58494)

## ETL Process
As stated above, the Data was extracted from DSA LMS and imported to Power BI for Transformation and Analysis.
In transforming the Data, NULL Values were removed from Salary and Department Columns, while Empty or blank spaces in the Gender column were replaced with ‘Others’ for unspecified Gender. To Achieved this, firstly I used TRIM to removed leading and trailing spaces from text strings, CLEAN to removed non-printable characters and lastly, the FIND and REPLACE to look for extra spaces and replacing with none. After which I then Replaced the empty Rows with ‘Others.’
The two Datasets (Palmoria Group emp-data.csv and Palmoria Group Bonus Rules.xlsx) were merged together after Transforming and Unpivoting the ‘Palmoria Group Bonus Rules.xlsx’ in order to have one single Table. After merging the Tables as one, one conditional column (Salary Band) and two custom columns (Bonus Amount and Salary + Bonus) were created.

## INSIGHTS BASED ON THE ANALYSIS
### KPIs
1.	Total Employees 946

2.	Female Count 441

3.	Male Count 465

4.	Others 40

5.	Total Salary $69.72M

6.	Average Salary $73.70K

7.	Maximum Salary $119.93K

8.	Minimum Salary $28.13K

### Dashboard Visuals
![PALMORA PROJECT DASHBOARD ](https://github.com/user-attachments/assets/7126ca76-973a-4e2b-9919-b7c565e4c68e)

## INSIGHTS AND RECOMMENDATIONS

### Gender Distribution in the organization
The Male Gender occupied 49.15% of the total employees in the organization over the Female with 46.62%. While the Unspecified (Others) Gender having 4.23%. Between the Male and the Female Gender, there is a gender gap difference of 2.53% of Male Employees over the Female Employees Company-wide.

### Gender Distribution Across Regions

#### Kaduna has 182 (49.86%) Male and 165 (45.21%) Female, giving a (4.65%) rise of Male Gender over the Female. While the Unspecified Gender (Others) have 18 (4.93%)

#### Abuja has 159 (48.04%) Male and 158 (47.73%) Female, giving a (0.31%) rise of Male Gender over the Female Gender. while the Unspecified Gender (Others) have 14 (4.23%)

#### Lagos has 124 (49.6%) Male and 118 (47.2%) Female, giving a (2.4%) rise of Male Gender over the Female. While the Unspecified Gender (Others) have 8 (3.2%)

### Recommendation 
There’s not much Gender distribution difference across the Region and the organization at large. However, to balance the little gap, more Female should be recruited into **Kaduna** and **Lagos Region**.

### Ratings based on Gender
The Male Gender has the Poorest Ratings. This could be due to family ties and other challenging factors associated with men.

### Recommendation 
More attention should be given to the Male Gender in order to know the caused of their poor performance.

### Company Salary Structure Analysis.
There is a Pay Gap difference of $0.04 Male Gender over the Female Gender. with the Female Gender being under paid across Departments and Region.

### Recommendation
Management should review the company salary structure in order to bridge the pay gap.

### Payment of $90,000 Minimum Salary to Employees
From the analysis, it was discovered that most of the Employees are paid below the new stipilated Minimum salary of $90,000, which falls short of the Industrial Standard Regulation as regards to the New Minimum salary payment.

### **Recommendation**
The management should work and ensure compliance with the new Industrial Regulation by effectively implementing the Nem Minimum Salary payment.

### Employees Payment Distribution by Group Band
   a)	$10,000 - $20,000: 	None
   
   b)	$20,000 - $30,000: 	    11 Female and 15 Male (26 Employees)
  
   c)	$30,000 - $40,000: 	    60 Female and 41 Male (101 Employees)
  
   d)	$40,000 - $50,000: 	    55 Female and 48 Male (103 Employees)
  
   e)	$50,000 - $60,000: 	    36 Female and 53 Male (89 Employees)
  
   f)	$60, 000 - $70,000: 	    40 Female and 54 Male (84 Employees)
  
   g)	$70,000 - $80,000: 	    56 Female and 54 Male (110 Employees)
  
   h)	$80,000 - $90,000: 	    57 Female and 48 Male (105 Employees)
  
   i)	$90,000 - $100,000: 	    None
   
   j)	$190,000+  		    126 Female and 152 Male (278 Employees)

   The above analysis on Group Band Payment is exclusive of the Unspecified Gender, Since of focus is on Gender Equality.
   
### The total amount to be paid to individual employees as Bonuses is **$2,199,279.30**. However, the amount allotted to individual employees can be seen on the Dashboard visuals.

### The total amount to be paid to individual employees as Bonus and Salary is **$71.92**.

### Total amount to be paid out per region and company-wide

##### KADUNA   $27.48M
##### ABUJA    $24.92M
##### LAGOS    $19.53M

### FOR THE COMPLETE PROJECT WORK, CLICK ON THE LINK BELOW
[https://drive.google.com/file/d/1eic6EvJ93SDhGQdWKrM3knXfFrc9g4LF/view?usp=drive_link]

### CONTACT ME
To reach out or connect with me, you can use the following channels:

LinkedIn [https://linkedin.com/in/valentineebi]

Email [ebivalentine6@gmail.com]

