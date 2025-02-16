# Q2-2021-Volume-Analysis
#GitHub Portfolio: Q2 2021 Volume Analysis
#Email Request
The board is asking to see how volume looks in Q2. I got some data gathered but didn’t have a chance to pull anything together and was hoping you could take a stab at it.
I think they just want to see the Q2 2021 volume by region and wanted to know if everything was looking good. I think this file has what you need. I don’t remember all the region codes – I know NAAM ends in 1, EMEA ends in 3, and APAC and LATAM are 2 and 4, but I don’t remember which is which. I do know LATAM has the lowest volume, so just go ahead and assign that to whichever comes out lowest.

#Data Cleaning Process
##Unwrapping Text
The data was wrapped together, making it difficult to read. I unwrapped it using the wrap/unwrap text ribbon in the Home button of Excel.
AutoFit Column Width
Used AutoFit Column Width in the Format ribbon to ensure data readability.

#Table Creation
Created a table using Ctrl + T and named it "Volume by Client", since it is a client volume dataset.
Checked for blanks using the filter option. No blanks were found.
Date and Number Formatting
The date column was in text format, so I used Text to Columns to convert it to a date format.
The volume column was also formatted as text, so I converted it to a number format.
##GeoID Dataset Cleanup
Applied similar formatting as the Volume Dataset.
Named the table "Geo by Client" as it represents Client Geography data.
Checked for duplicates and blank values in Client ID – none were found.
The GeoID column had duplicates, so I copied it to another sheet and removed duplicates, obtaining:
Geo001 - NAAM
Geo003 - EMEA
Geo002 - (Unassigned)
Geo004 - (Unassigned)
Solving the LATAM & APAC Region Mapping
The email indicated LATAM has the lowest volume.
Used SUMIFS() to find the lowest volume and assigned it to LATAM, then assigned the second lowest to APAC.
Final Assignments
Geo001 - NAAM - 3,002,286
Geo003 - EMEA - 830,760
Geo002 - APAC - 562,005
Geo004 - LATAM - 425,262
Combining the Data: Merged all datasets into one worksheet using XLOOKUP() to assign region names.
Discoveries Using Pivot Table
Customer Attrition in LATAM: Two customers left the LATAM region in Q2, resulting in a 7k volume loss.
Q2 Growth Analysis: Q2 growth slowed from 4% in Q1 to 2.7%. The primary cause was the 7k volume decline from LATAM customer attrition. LATAM growth declined from 9% in Q1 to flat in Q2 (YoY). NAM Region Client Onboarding Impact Q2 2020 NAM client onboarding anniversaried in Q2 2021. This led to a slowdown in perceived growth.
#Conclusion
The data analysis reveals critical insights into Q2 2021 volume trends. The LATAM region experienced customer attrition, impacting overall growth, while the NAM region faced a slowdown due to anniversary effects. These insights can help inform strategic decisions for upcoming quarters.
#Next Steps
Investigate further customer churn reasons in LATAM.
Develop customer retention strategies to mitigate future losses.
Assess onboarding strategies in NAM to sustain growth momentum.

This structured approach demonstrates a strong ability to analyze business data, use Excel functions effectively, and present findings in a clear and actionable format. GitHub Portfolio: Q2 2021 Volume Analysis

