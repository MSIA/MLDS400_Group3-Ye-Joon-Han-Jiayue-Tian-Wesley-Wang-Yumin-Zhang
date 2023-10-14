**Updates: (Oct 8th-Oct 13th)**

* Created a GitHub repository accessible to four team members, a TA, and Professor Diego
*	Installed pgAdmin, established a connection to the MLDS Postgres server, and conducted an initial exploration of the pgAdmin interface
* Established the tables in PostgreSQL (deptinfo, skstinfo, strinfo) according to the database schema and provided access to all team members (Note: we faced issue importing the other two tables because of ambiguous column label and mismatch between the number of columns in the schema and the actual dataset.)
* Summary Statistics:	Mean, Min, Max, SD of “COST”, “RETAIL” in table skstinfo

Summary Statistics (more):
*	Found a lot of problems with the data, including incomplete foreign keys and poorly defined and duplicated columns in trnsact. 
*	In particular, the last (undeclared) column of each table has columns of 0 and 1. 
*	Total 787669 distinct SKU inside the skuinfo table. 
*	Shown the Top 5 Most Profitable Stock Items, sum(retail) - sum(cost)

![image](https://github.com/MSIA/MLDS400_Group3-Ye-Joon-Han-Jiayue-Tian-Wesley-Wang-Yumin-Zhang/assets/145066585/da7b89f8-82ac-4d4e-9496-c234948de2f8)

*	Figured the Top 5 busiest store in the US (based on counting the number of stock item)

![image](https://github.com/MSIA/MLDS400_Group3-Ye-Joon-Han-Jiayue-Tian-Wesley-Wang-Yumin-Zhang/assets/145066585/ad6286ac-5d86-4d60-b7b7-748b5579d460)


**Next Steps: (Oct 16th-Oct 21st)**

* Understand, clean, and import the other two tables (skuinfo, trnsact) into PostgreSQL
*	Explore data and the table relationship and do some EDA

