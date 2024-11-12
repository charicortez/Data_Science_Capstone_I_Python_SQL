# **Attrition in IBM: Investigating the impact of employee work-life balance**
____________________________
##  Background 
<img width="477" alt="Screenshot 2024-11-12 at 12 51 06 PM" src="https://github.com/user-attachments/assets/21d66eb6-292b-41ee-8b0c-8792b728064c">

In this project, I investigated potential factors that led to employee attrition using the [IBM HR Analytics Employee Attrition & Performance dataset](https://www.google.com/url?q=https%3A%2F%2Fwww.kaggle.com%2Fdatasets%2Fpavansubhasht%2Fibm-hr-analytics-attrition-dataset). High attrition results in open positions, gaps in critical knowledge and skill sets, and unfulfilled work. These deficits lead to increased burden and workload on existing/current employees, which likely result in employee burnout and increased attrition. 
According to the [Academy to Innovate HR](https://www.google.com/url?q=https%3A%2F%2Fwww.aihr.com%2Fblog%2Femployee-attrition%2F), relevant stakeholders can use "**data-driven approaches**" to "help companies determine what's causing employees to leave...Then, they can target those issues and really work to keep people around."

## Introduction
<img width="382" alt="Screenshot 2024-11-12 at 1 48 18 PM" src="https://github.com/user-attachments/assets/a4eb258c-c39f-4b43-ae18-1e856ef42535">

This dataset provides a variety of information for both current and former employees, including education level, job satisfaction, distance from work, department, and score for work-life balance. Although this is a fictional dataset based on IBM, a reality across many industries is that innovation is the lifeblood of any successful company. In order to *quantify and better understand employee attrition*, I will address the folowing questions:

- What is the size of the company and each of its departments?
- What is the overall attrition rate for each department?
- What is the relationship between work-life balance and department for both current employees and former employees?
- Is there a statistically significant difference in the score given for work-life balance between current employees and former employees?

Knowing the attrition rates is imperative, as [an attrition rate exceeding 10% could be problematic for the company](https://www.google.com/url?q=https%3A%2F%2Fhttps%3A%2F%2Fwww.indeed.com%2Fhire%2Fc%2Finfo%2Femployee-attrition).

Analysis of data from all three departments will be provided because all attrition rates– for the company overall and by each department–should be known. However, I will focus on R&D, as it is often the largest and typically the department responsible for creating and developing the company’s products.

## Hypotheses
H₀: There is *no statistically significant difference* between the average work-life balance score between former R&D and current R&D employees.

Hₐ: There is *a statistically significant difference* between the average work-life balance score between former R&D and current R&D employees.

## The Data
- 1,470 records
- 35 variables
- Clean
- Not longitudinal 
![image](https://github.com/user-attachments/assets/35992b6b-432c-4775-8dbe-f253b036ee9c)

## Methods
1. Form two dataframes based on attrition
2. Calculate overall attrition rate
3. Create sub-groups based on attrition and department
4. Calculate departmental attrition rate
5. Analyze work-life balance data
6. Determine statistical significance

<img width="338" alt="image" src="https://github.com/user-attachments/assets/d39125ca-fd3e-4520-abbf-590831434090">

## Results

### All departmental rates of attrition are >10%
<img width="572" alt="image" src="https://github.com/user-attachments/assets/2a107c01-e7b7-4869-839c-3d6e5ebc0e21">

### HR work-life balance data are not normally distributed; similar mean work-life balance score from current and former employees
<img width="692" alt="image" src="https://github.com/user-attachments/assets/87337d1c-08db-4c26-b502-3d15472a03f4">
<img width="621" alt="image" src="https://github.com/user-attachments/assets/9b984c46-1f56-4801-86cc-8cc66417769c">

### Sales work-life balance data are not normally distributed; lower work-life balance score from former employees
<img width="696" alt="image" src="https://github.com/user-attachments/assets/cfe08de3-bae3-4c97-9ae1-6ee4247ba9f0">
<img width="621" alt="image" src="https://github.com/user-attachments/assets/c6f2eb96-d434-4e8d-a0e6-e7248be8c544">

### R&D work-life balance data are not normally distributed; lower mean work-life balance score from former employees
<img width="696" alt="image" src="https://github.com/user-attachments/assets/ca07a453-4128-4a49-93ee-aa5f0fbb274e">
<img width="621" alt="image" src="https://github.com/user-attachments/assets/71406f99-c860-4b0d-ae00-241ceb33d874">

### The Kruskal-Wallis test was used to determine statistical significance
<img width="344" alt="image" src="https://github.com/user-attachments/assets/b4a46e3a-da64-4cc6-b8f9-2cdb1c8e1165">

</n><img width="334" alt="image" src="https://github.com/user-attachments/assets/397e580e-f5eb-40e0-b858-ed657326ef09">

## Reject the null hypothesis 
<img width="419" alt="Screenshot 2024-11-12 at 2 17 38 PM" src="https://github.com/user-attachments/assets/32037892-a2a1-4e92-9703-418ad09a0b21">

## Improving the work-life balance in R&D will likely reduce attrition
- The overall attrition rate is 19%, which is nearly double the target rate of 10%
- All departmental attrition rates *exceeded 10%*
- *R&D attrition accounts for 56.1% of overall attrition*
  - Of the 237 employees that left the company, 133 of those employees were R&D
- **The difference in R&D work-life balance means is statistically significant**
  - Strongly suggests that efforst to improve work-life balance in R&D will likely improve employee retention and reduce the attrition rate
 
## Follow-up studies to further characterize R&D attrition would be beneficial 
<img width="277" alt="image" src="https://github.com/user-attachments/assets/475aa2bf-91cd-440b-b05c-c53dfeec5d00">

The majority of R&D attrition occurs within the first year of employement. This attrition [equates to roughly $180,000 - $900,000 (not including salary and benefits) in immediate failed monetary investment](https://github.com/user-attachments/assets/48c72f12-054c-4466-a749-6b180c3c61d9). These data suggest the need to improve critical hiring procedures in order to improve employee retention.

## This study has provided a clear, more specific target to improve employee retention
The results of this study show that the company has problematic attrition rates that need to be addressed. This study has provided a more *specific target for relevant stakeholders to address then implement improvements*. Improvements in work-life balance will reduce attrition and maintain operational efficiency.

<img width="556" alt="image" src="https://github.com/user-attachments/assets/9b6b728a-1b74-4880-8b3f-cf91eb031d9b">







