# motor-vehicle-crashes
Data Management Project, end-to-end Data Engineering and Visualization

Link for metadata - https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes

Scope:
The scope of this project includes analyzing the dataset, loading the data into Snowflake, and producing fact and dimension tables to allow you to generate SQL query to produce the KPI. 
The KPIs will then be represented in Tableau dashboards. 
The Tableau dashboard should be customizable, allowing to select different dimensions to observe data. 
The final deliverable for this project will be a project report and a Tableau dashboard.
To complete this project, students should demonstrate experience in data analytics, database management, and data visualization. They should use strong communication skills and be able to work collaboratively together to ensure that the final deliverable meets all requirements.
Upon completion of this project, the student team will have gained valuable experience in data management and analytics. 
Additionally, they will be able to shared their work on social media like LinkedIn or during interviews.

Recommended Steps:
1. Load the dataset into Snowflake (you can either copy the file to your S3 bucket or try to load directly from Snowflake from your desktop). Describe which method you used and why.
2. Build a Data Dictionary of the dataset (look for the Metadata Source on the crime data dataset page on the data.gov web site, link above.
3. Dimensional Modeling
    a. Define the business or event process.
    b. Define the grain.
    c. Define your Fact and Dimensions to produce the necessary KPIs listed below using the 7Ws (who does what, when …)	
4. Build the Fact and Dimension tables
    a. Provide an ERD Diagram of your fact and dimension tables (a star schema showing the relationship between the tables and the column names). 
    b. I recommend DBSchema (https://dbschema.com/) but you’re free to use any other tools. (Another one is Navicat)
5. Generate your Fact and Dimension in your Snowflake account using SQL.
6. Populate your fact and dimension tables using SQL (date_dim, timeOfday_dim if necessary), and other necessary dimensions for your analytics.
7. Write the SQL query to generate the KPIs below.
8. Connect Tableau to your Snowflake account, and build 5 dashboards to represent the different KPIs below.
9. Use the Tableau dashboards you have built to provide analytical observation as if you were presenting this data visualization to the Mayor of New York. 
    a. Try to extract some important insights ; to tell a story.

KPIs:
1. Crashes by area: This KPI measures the number of crashes by zip code/borough, on a given period of time (e.g. month, quarter, year, etc.). 
2. Number of people injured by Contributing Factor: This KPI measures the number of people injured in the accident for each type of contributing factor (e.g. unsafe speed, pavement slippery, etc.). It can be calculated for a given period of time.
3. Number of people killed by Contributing Factor: This KPI measures the number of people killed in the accident for each type of contributing factor (e.g. unsafe speed, pavement slippery, etc.). It can be calculated for a given period of time.
4. Injuries/Deaths per type of vehicle in the crash: This KPI measures the number of injured people by the combinations of the type of vehicles involved e.g. (van&bike, sedan&bus, etc.). It can be calculated for deaths instead of injured people. It can be calculated for a given period of time. 
5. Injuries/Deaths vs Crashes rate: This KPI measures the percentage rate between people injured and the number of crashes. It can be calculated as (# people injured/ # crashes) * 100 (or killed instead of injured) for a given borough, zip code and/or time period. It can be calculated for deaths instead of injured people as well.

Project Report:
The project report includes the following:
1. Executive Summary: A brief and concise summary of the project, highlighting the most critical and relevant insights and findings.
2. Project Statement: Project introduction showing a clear understanding of the dataset and the project goals.
3. Data Dictionary: Structured description of the data elements, attributes, and entities present in the data warehouse (tables and relationships, attributes, data types, lengths, domains, and constraints)
4. Dimensional Modeling + ERD
Use the 4 critical steps learnt in class to define your fact and dimension tables.Represent your fact and dimension tables in a star schema. Explain why you choose these dimensions. What are the measures? Paste your star schema in the document. 
5. Data Transformation: Explain how you populated your dimensions and fact table. Don’t paste long SQL into the document. Store your SQL command in a SQL file and add to the folder.
6. Produce KPIs using Fact and Dim: Explain which dimension and fact you use to generate each KPIs. If SQL is few lines you may copy in the document. Include your SQL also in a separate file and store in the folder. 
7. Data Visualization: Show your dashboards (screenshot) and provide analytical observation. Try to extract some important insights, to tell a story. Maybe make a list of recommendations or actions. 
8. Project Challenges: Brief summary of the project limitations, challenges faced, and how you solved them. 
