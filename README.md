**Updates: (Oct 8th-Oct 13th)**
<br /> ●	Created a GitHub repository accessible to four team members, a TA, and Professor Diego
<br /> ●	Installed pgAdmin, established a connection to the MLDS Postgres server, and conducted an initial exploration of the pgAdmin interface
<br /> ●	Established the tables in PostgreSQL (deptinfo, skstinfo, strinfo) according to the database schema and provided access to all team members (Note: we faced issue importing the other two tables because of ambiguous column label and mismatch between the number of columns in the schema and the actual dataset.)
<br /> ●	Summary Statistics:
<br /> 1.	Mean, Min, Max, SD of “COST”, “RETAIL” in table skstinfo
<br /> Summary Statistics:
<br /> ●	Found a lot of problems with the data, including incomplete foreign keys and poorly defined and duplicated columns in trnsact. 
<br /> ●	In particular, the last (undeclared) column of each table has columns of 0 and 1. 
<br /> ●	Total 787669 distinct SKU inside the skuinfo table. 
<br /> ●	Shown the Top 5 Most Profitable Stock Items, sum(retail) - sum(cost)
<br /> <img width="203" alt="image" src="https://github.com/MSIA/MLDS400_Group3-Ye-Joon-Han-Jiayue-Tian-Wesley-Wang-Yumin-Zhang/assets/145531369/2631a4a2-485d-4148-a752-9545d954b0f9">
<br /> ●	Figured the Top 5 busiest store in the US (based on counting the number of stock item)
<br /> <img width="327" alt="image" src="https://github.com/MSIA/MLDS400_Group3-Ye-Joon-Han-Jiayue-Tian-Wesley-Wang-Yumin-Zhang/assets/145531369/6ff399d1-6d86-43e0-9f33-d879f49b4bf6">

<br /> Next Steps: (Oct 16th-Oct 21st)
<br /> ●	Understand, clean, and import the other two tables (skuinfo, trnsact) into PostgreSQL
<br /> ●	Explore data and the table relationship and do some EDA
