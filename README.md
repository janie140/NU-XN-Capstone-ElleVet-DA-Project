# NU-XN-Capstone-ElleVet-DA-Project
This project aimed to analyze ElleVet’s transaction data to address key business questions regarding customer behavior, lifetime value (LTV), and customer acquisition strategies.

Our analysis focused on understanding purchase patterns, customer segmentation, and how these insights could inform business decisions.

*The deliverables for this project include:
1.	A PowerPoint presentation summarizing the analysis, visualizations, and insights derived. Proposals for future projects, including recommendations for additional analyses or initiatives to pursue.
2.	Individual code files used for the analyses. 
3.	This summary document, which outlines the questions tackled by each team member, datasets used, and the associated code files.
   
*Dataset Overview
Our analysis is based on two primary datasets provided by Eleevet:
1.	‘EVS_sept24Data.csv’:
A sample of 6,398 rows representing customer transactions, including subscribers and one-time buyers.
2.	Roux_Active_Vet_File.xlsx:
A workbook of veterinary-related data, including transaction records from 2022–2024, a "Top 100 Vets" list, and additional details on veterinary clinic activity.

*My contribution:
Question Explored: How can we use data to understand, deconstruct, and improve the connection between vets and consumers: we know that 70% of consumers identify a veterinarian’s recommendation as the reason for trying ElleVet. But currently we do not have levers in use to expedite the time it takes vets and consumers to find one another. There are five cohorts that exist in a geography:

1. There are ß vets who carry ElleVet and recommend it
2. There are Z vets who do not carry ElleVet BUT recommend it.
3. There are ∂ existing customers in the geography who currently use ElleVet
4. There are µ vets who have never carried ElleVet/never heard of it
5. There are X pet owners who have never tried ElleVet/never heard of it
   
How do we use geotagging, data science, analytics, to identify members of these cohorts, and facilitate interaction so that: ß+Z+∂ => X+µ, where =>is a factor applied to bring these cohorts into contact with one another and stimulate adoption and acceptance. What are those force factors that can be applied? How do we apply them?

**Methods:
•	Cross-Analysis: Preprocess, filter, reclassify customer roles and merge two datasets "All transactions" and "Vets' transactions".
•	Geospatial Analysis: Map the concentration of ElleVet consumers and vets using their geolocation data and geocoding techniques.
•	Cluster Analysis: Use clustering algorithm DBSCAN to quantify concentrations of ∂ consumers and β clinics and highlight areas with unmet demand.
•	Predictive Analysis: Propose a propensity model to infer Z clinics who recommend but not carry ElleVet.

**Key Findings:
•	An interactive map used to assess the density of existing consumers with existing vets in each specific area.
•	Precise identification of high-density regions and actionable metrics for targeted outreach or marketing, such as the number of clusters, size of each cluster, and density of consumers/vets in each.
•	Predictive model development: Conducted feature engineering and proposed a classification model concept (propensity model) to infer Z Clinics.

**Limitations:
•	Limitation on tracking consumer data (referrals, demographic features, feedback, etc) and the connection between consumers – referral programs – vets.
•	No unpaid or public data sources about Pet Ownership rate/population and Clinic Density per area were found.
•	Not enough data for training the predictive model (need non-Ellevet clinic list and other survey data)
