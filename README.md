<a name="top"></a>
# Cancer Prevention-Regression Analysis (The African Cancer Institute)
---

> <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228323145-dc1343c4-a9e5-4e15-ae91-8af1bc9898b8.svg"> **Author:** Richard Taracha 

> <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228325498-2a141e3e-3e77-48b0-96ae-cbfffa4ef2b3.svg"> **Date:** 23/10/2023

<!-- > <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228318759-abcf91d4-5ddd-4230-aed8-4c8d7f63f8d2.svg"> **Web Application:** <a href="https://cancer-deathrate-regression-analysis.onrender.com" target="_blank">Click Me!</a> -->

<!-- <img align="right"  width="450" height="350" src="https://user-images.githubusercontent.com/67068918/107158150-3977d700-6999-11eb-9603-63f72f2741a9.png"> -->
<img align="right" width="600" height="338" src="https://github.com/TarachaR/Credit-Risk-of-Mobile-Loan-Applicants/assets/67068918/03370bb3-9d5d-41eb-ac6b-f099b8ea09a2">

---
</br>


> ### <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228328212-52e66179-e80d-4416-906d-64e401ce7052.svg"> Table of Contents
- [Background Information](#background-information)
- [Understanding The Context](#understanding-the-context)
- [Project Deliverable](#project-deliverable)
- [Recording the Experimental Design](#recording-the-experimental-design)

</br>

---

</br>

> ## <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228328828-3d2fa345-dc76-44c6-a604-5a05aeea636b.svg"> Comprehending The Setting
***Safaricom, a telecommunications behemoth with deep roots in Kenya, has carved a niche for itself in the realm of financial services through its M-PESA brand. M-PESA, transcending its origins as a mere mobile money transfer platform, has evolved into a comprehensive financial ecosystem catering to the diverse needs of millions of Kenyans.***

***At the heart of M-PESA's success lies its ability to provide a secure and convenient means of transferring funds between individuals. This has not only revolutionized the way Kenyans conduct their daily financial transactions but has also played a pivotal role in promoting financial inclusion among the unbanked and underbanked segments of the population.***

***In 2013, Safaricom, in a strategic partnership with CBA, launched M-SHWARI, a savings and loan product designed to tap into the vast potential of the M-PESA user base. M-SHWARI has since grown into a formidable force in the Kenyan microfinance landscape, providing millions of Kenyans with access to affordable and readily available credit.***

***M-SHWARI loans are typically small in size and have a short repayment period of 30 days. This makes them ideal for meeting short-term financial needs such as medical emergencies, school fees, and business expenses. The convenience of accessing M-SHWARI loans through the M-PESA platform has made it a popular choice among Kenyans seeking quick and hassle-free access to credit.***

***In addition to M-SHWARI, Safaricom also offers Okoa Jahazi, a credit loan service for prepaid subscribers. Okoa Jahazi allows subscribers to access small loans that are repaid through automatic deductions from their airtime top-ups. This service has proven to be a lifeline for many Kenyans who find themselves in need of immediate cash during times of financial difficulty.***

***Safaricom's foray into the financial services sector has been nothing short of remarkable. Through M-PESA, the company has not only provided Kenyans with a convenient and secure means of conducting financial transactions but has also played a major role in promoting financial inclusion in the country. As Safaricom continues to innovate and expand its financial services offerings, it is poised to play an even greater role in shaping the future of finance in Kenya.***
</br>

Source: https://www.businessdailyafrica.com/bd/economy/half-mobile-phone-borrowers-default-3654550

---

> ## <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228328828-3d2fa345-dc76-44c6-a604-5a05aeea636b.svg"> Data Pertinence and Attribution
In December 2021, a household survey conducted by Central Bank of Kenya (CBK), FSD Kenya and the Kenya National Bureau of Statistics (KNBS) revealed that 50.9% of mobile loan borrowers had defaulted on their loans. The survey also found that 12.5% of mobile loan borrowers had defaulted on their loans more than once. This is a worrying trend that needs to be addressed if Kenya is to achieve its goal of becoming a middle-income country by 2030.

> ## <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228329440-1b010e60-3ec5-4d81-b545-ef3991a6eb95.svg"> Understanding The Context

As a Data Scientist working for the institution you have been tasked to identify factors that contribute to loan default. The findings of your analysis will be used to inform the creation of a credit scoring model that will be used to determine the creditworthiness of Okoa Jahazi loan applicants. The model will be used to predict whether or not an applicant will default on their loan based on their credit history and other relevant factors. This will help the institution make better lending decisions and reduce the number of loan defaults.

> ## <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228329440-1b010e60-3ec5-4d81-b545-ef3991a6eb95.svg"> Formulating the Benchmark of Success

**The project’s objective is to estimate when a person will default on their loan. We construct a model that incorporates all the relevant data to reliably predict the outcome.**

**Loan defaulting occurs when a person does not fulfill their debt obligation in the specified period. A loan is considered to be in default for risk modelling purposes if it is more than 90 days old.**

**We will have achieved our objective when we get at least one model with an accuracy score of around 80%.**

#### Technologies and Tools: Python, Pandas, Numpy, Matplotlib, Scikit-Learn

<p align="right"><a href="#top">Back to top</a></p>

---

> ## <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228330000-aab764a7-0178-4536-b3f9-50fa169afe63.svg"> Project Deliverable
There are three deliverables for this project:
- A **GitHub repository**
- A **Jupyter Notebook**
- A **non-technical presentation**
</br>
</br>


<h4 align="center">Dataset Attributes:</h4>

| CUST_TXN_DATE | Customer Transaction Date |
|-|-| 
| CUST_ID_ACCT1 | Account Identifier |
| DEPOSIT_AMNT_MPSA | Amount deposited on Mpesa |    
| RCVD_AMNT_MPSA | Amount received on Mpesa |
| TRSF_FROM_BANK_TO_MPESA_AMNT | Amount on transfers from Bank on Mpesa |  
| MPSA_CREDITS | Mpesa credits |
| DAYS_ARTM_LESS_2 | Number of days airtime is less than 2 |
| X_NR_TOT_LOAN_AMNT_OKOA_JAZI | Total loan amount on okoa jahazi |
| LOAN_AGE_DAYS | Loan age in days |


<p align="right"><a href="#top">Back to top</a></p>

---

> ## <img align="left" width="25" height="25" src="https://user-images.githubusercontent.com/67068918/228331342-873c97d4-48bf-49e6-992e-788202af2cd3.svg"> Recording the Experimental Design
The following steps were followed during the implementation of the project:

| Step | Task |
|-|-|  
| 1 | Define the Research Question. |
| 2 | Data Importation. |
| 3 | Data Exploration. |   
| 4 | Data Cleaning. |
| 5 | Exploratory Data Analysis |
| 6 | Data Preparation |
| 7 | Data modelling. |
| 8 | Model Evaluation. |
| 9 | Summary of Findings |
| 10 | Recommendations / Conclusions |
| 11 | Challenge solution. |



<p align="right"><a href="#top">Back to top</a></p>

---

<h3 align="center">Made with ❤️ by Richard Taracha</h3>


