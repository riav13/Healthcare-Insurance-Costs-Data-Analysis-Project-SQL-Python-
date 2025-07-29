Healthcare-Insurance-Exploratory-Data-Analysis-with-SQL
## Dataset Source: https://www.kaggle.com/datasets/willianoliveiragibin/healthcare-insurance
## Author: Ria Verma
## Tools/Languages Used: SQLite, SQL,Python, Jupyter Notebook (optional), Microsoft Excel

## Goal: The goal of this project is to investigate patterns in US healthcare insurance costs by using a mix of basic and intermediate SQL queries I learned through IBM certiifcation. I analyzed a dataset fro Kaggle which contained over 1,300 individual records. For this exploratory data analysis project, my primary focus was to understand how variables such as age, gender, smoking, region, and family size influence healthcare costs. I wanted to practice my sql/ python for data visualization and this was my first EDA project where I uncovered insights that are directly relevant to business decisiosn making in the insurance/healthcare industry.

------------------------------------------------------------------------------------------------------------------------------
## Dataset Summary

The dataset includes 7 attributes/primary keys: age, sex, body mass index (BMI), number of children, smoking status (yes/no), region (northeast, southeast, northwest, southwest), and insurance charges. Each record represents an individual, and the charges column reflects the medical cost billed to the insurance company. This dataset provides insight into the types of variables that drive healthcare costs and insurance risk.

----------------------------------------------------------------------------------------------------------------------------
## Key Findings and Insights

To begin, I calculated general statistics such as the average, minimum, and maximum charges across the dataset. The average medical charge was $13,260, with a wide range spanning from just over $1,000 to more than $60,000. This large spread suggests the presence of high cost outliers, potentially tied to health issues and risky behaviors like smoking.

The gender distribution in the dataset is even with almost a 1:1 ratio of males to females. When analyzing the average charges by gender, I found that males tend to have slightly higher insurance costs than females, though the difference was not dramatic. This finding may be influenced by other overlapping factors like age and smoking status.

** One of the clearest trends emerged when analyzing the impact of smoking. Smokers in the dataset pay much more in healthcare charges than non smokers. On average, smokers have over $23,000 more in insurance costs. This aligns with the known health risks associated with smoking and reflects why insurance providers might price higher for smokers. 
Among individuals who pay more than the average charge, a notable portion are non smokers which indicates that other variables like age and BMI could also contribute to elevated costs.

The relationship between age and charges was also clear. As age increases, insurance costs generally rise as well. Most of the individuals with above average charges fall into the age range of 50 to 64, likely due to the increasing prevalence of chronic conditions and healthcare needs with age.

When comparing charges by region, I discovered that the southeast region had the highest average charges, while the southwest had the lowest. This regional variation may be due to differences in population health or healthcare access. Maybe this suggests that insurers should consider regional trends when developing pricing strategies for insurance.

In examining family size, I found that individuals with more children tended to have lower average charges. This is most likely due to differences in the types of family insurance coverage plans selected. It is an important factor for insurers to consider when considering family plans.

To identify high cost outliers, I queried the top 5 individuals with the highest charges. They were all in their 50s or older, many were smokers, and most had elevated BMIs which demonstrated a clear link between lifestyle risk factors and extreme costs. In another set of queries, I filtered records using subqueries to identify people paying above and below the average charge. Among those below average, most were older females who did not smoke, while those above were typically middle aged males and smokers with no or few children.

Finally, I compared the number of smokers and non smokers who are paying more than the average charge. Although smokers represent the highest individual charges, the majority of people paying above average were actually non smokers, showing that age and BMI likely still play a substantial role, even if a person doesn't smoke.

-----------------------------------------------------------------------------------------------------------------------------


The insights from this analysis are directly applicable to a real world insurance company. Risk based pricing strategies can be better informed by understanding how smoking, age, and region correlate with higher costs. For example, people who are older or smoke may pay higher prices based off of their risk profile. I also found that the southeast region has higher average costs which could be a coincidence but could also result in more targeted policy changes/investigating deeper. The finding that larger families often have lower costs might influence new considerations of family coverage plans. Ultimately, this project demonstrates how structured data and SQL analysis can drive smarter pricing, risk assessment, and other strategies.

----------------------------------------------------------------------------------------------------------------

## Conclusion

This project helped me practice my SQL querying data skills, but also the ability to critically analyze and interpret data in a way that leads to actionable business insights which is something I am trying to learn. Through structured queries, subqueries, grouping, and filtering, I was able to uncover patterns that could be valuable for a real scenario. Beyond just querying the data, I wanted to understand it to identify key trends to help me draw real world conclusions. 


