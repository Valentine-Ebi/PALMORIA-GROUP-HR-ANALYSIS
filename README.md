# PALMORA GROUP HR ANALYSIS 
## PROJECT OVERVIEW 
Palmoria Group, a manufacturing company based in Nigeria, has recently come under scrutiny over concerns of gender inequality across its regional operations. The situation escalated following a media report labelling the organization as “Palmoria, the Manufacturing Patriarchy.” In response, the company’s leadership mandated a comprehensive review of its human resources data to uncover potential biases and address them proactively.

As an HR Analytics Consultant, I was engaged to perform a deep-dive analysis of Palmoria’s employee data. The focus was to uncover insights related to gender distribution, performance ratings, pay disparities, and bonus allocations, especially through the lens of gender equity and regulatory compliance.
This project uses Power BI to visualize and analyze key HR metrics to support data-driven decision-making at Palmoria Group.

## Project Objectives
1.	Data Cleaning and Preparation:

  	 a).	Handle missing values in gender, department, and salary.

  	 b).	Exclude non-active employees and undefined departments.

  	 c).	Standardize bonus rules for analysis.

3.	Gender-Based Insights:

  	a).	Analyze gender distribution by region and department.

  	b).	Identify any gender bias in employee performance ratings.

  	c).	Visualize representation gaps in the workforce.

5.	Salary & Pay Gap Analysis:

  	 a).	Investigate the existence and extent of a gender pay gap.

  	 b).	Identify departments or regions where disparities are most pronounced.

7.	Compliance Evaluation:

  	 a).	Evaluate adherence to a regulatory minimum salary requirement of $90,000.

  	 b).	Visualize salary band distribution across the organization.

9.	Bonus Allocation & Impact:

  	a).	Apply department-based bonus rules to employee ratings.

  	b).	Calculate individual and regional bonus payouts.

  	c).	Evaluate the financial impact of bonuses on total compensation.

11.	Dashboard Design:

   	 a).	Develop an interactive Power BI dashboard with KPIs, charts, and tables.

   	 b).	Enable management to explore insights by gender, department, and location.


## Data Source
The data for this Analysis was gotten from Digital SkillUp Africa (DSA) Learning Management System (LMS) as part of my final project.

## Tools Used for the Analysis
The tool for this is Power BI. You can download it via this link (https://www.microsoft.com/en-us/download/details.aspx?id=58494)

## ETL Process
As stated above, the Data was extracted from DSA LMS and imported to Power BI for Transformation and Analysis.
In transforming the Data, NULL Values were removed from Salary and Department Columns, while Empty or blank spaces in the Gender column were replaced with ‘Others’ for unspecified Gender. To Achieved this, firstly I used TRIM to removed leading and trailing spaces from text strings, CLEAN to removed non-printable characters and lastly, the FIND and REPLACE to look for extra spaces and replacing with none. After which I then Replaced the empty Rows with ‘Others.’
The two Datasets (Palmoria Group emp-data.csv and Palmoria Group Bonus Rules.xlsx) were merged together after Transforming and Unpivoting the ‘Palmoria Group Bonus Rules.xlsx’ in order to have one single Table. After merging the Tables as one, one conditional column (Salary Band) and two custom columns (Bonus Amount and Salary + Bonus) were created. Measures were also created to calculate Gender Pay Gap. etc

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

![Dashboard V](https://github.com/user-attachments/assets/c2c8f4b8-ebe4-45a5-a0df-0de1e248ea21)

![Gender Gap by Region and Department](https://github.com/user-attachments/assets/e4293ff5-76a2-4bca-9ca4-b4e0d2469d86)

## INSIGHTS AND RECOMMENDATIONS

### 1.0        Gender Distribution in the organization
The Male Gender occupied 49.15% of the total employees in the organization over the Female with 46.62%. While the Unspecified (Others) Gender having 4.23%. Between the Male and the Female Gender, there is a gender gap difference of 2.53% of Male Employees over the Female Employees Company-wide.

### 1.0        Gender Distribution Across Regions

#### Kaduna has 182 (49.86%) Male and 165 (45.21%) Female, giving a (4.65%) rise of Male Gender over the Female. While the Unspecified Gender (Others) have 18 (4.93%)

#### Abuja has 159 (48.04%) Male and 158 (47.73%) Female, giving a (0.31%) rise of Male Gender over the Female Gender. while the Unspecified Gender (Others) have 14 (4.23%)

#### Lagos has 124 (49.6%) Male and 118 (47.2%) Female, giving a (2.4%) rise of Male Gender over the Female. While the Unspecified Gender (Others) have 8 (3.2%)

### Recommendation 
There’s not much Gender distribution difference across the Region and the organization at large. However, to balance the little gap, more Female should be recruited into **Kaduna** and **Lagos Region**.

### 2.0        Ratings based on Gender
The Male Gender has the Poorest Ratings. This could be due to family ties and other challenging factors associated with men.

### Recommendation 
More attention should be given to the Male Gender in order to know the caused of their poor performance.

### 3.0        Company Salary Structure Analysis.
At Palmoria Group, the overall Gender Pay Gap is 3.55%, indicating that, on average, female employees earn 3.55% less than their male counterparts.
This is a relatively small gap, but still significant and worth monitoring, especially considering Palmoria’s recent reputation concerns.

### Gender Pay Gap by Department
Most departments have a positive pay gap, meaning men earn more. However, Marketing and Engineering show a reverse gap, indicating women are paid more than men on average in those departments.

Gender-based salary inequality exists more in HR, Business Development, and Services.
Conversely, Engineering and Marketing departments exhibit a reverse pay gap.

### Gender Pay Gap by Region
Gender pay gaps are present in all regions but remain within the 3–4% range, suggesting regional policies or practices are relatively balanced.

Regional gaps are modest and likely driven by departmental composition or role types rather than systemic issues.

### 4.0        Payment of $90,000 Minimum Salary to Employees
From the analysis, it was discovered that most of the Employees are paid below the new stipilated Minimum salary of $90,000, which falls short of the Industrial Standard Regulation as regards to the New Minimum salary payment.

### **Recommendation**
The management should work and ensure compliance with the new Industrial Regulation by effectively implementing the Nem Minimum Salary payment.

### 4.1        Employees Payment Distribution by Group Band
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
   
### 5.0        The total amount to be paid to individual employees as Bonuses is **$2,199,279.30**. However, the amount allotted to individual employees can be seen on the Dashboard                    visuals.

### 5.1        The total amount to be paid to individual employees as Bonus and Salary is **$71.92**.

### 5.2        Total amount to be paid out per region and company-wide

##### KADUNA   $27.48M
##### ABUJA    $24.92M
##### LAGOS    $19.53M

## Conclusion
The HR analytics dashboard created for Palmoria Group equips the leadership team with actionable insights to address gender-related concerns proactively. Through this project, critical issues such as unequal gender representation, pay disparity, and rating biases have been made transparent using visual storytelling.

Beyond internal reform, the project supports Palmoria’s ambitions for global expansion by aligning its HR practices with inclusive, equitable, and compliant standards. With the right strategic actions, Palmoria can move from controversy to becoming a model for progressive HR management in the manufacturing sector.


### FOR THE COMPLETE PROJECT WORK, CLICK ON THE LINK BELOW
[https://drive.google.com/file/d/1eic6EvJ93SDhGQdWKrM3knXfFrc9g4LF/view?usp=drive_link]

### CONTACT ME
To reach out or connect with me, you can use the following channels:

LinkedIn [https://linkedin.com/in/valentineebi]

Email [ebivalentine6@gmail.com]

