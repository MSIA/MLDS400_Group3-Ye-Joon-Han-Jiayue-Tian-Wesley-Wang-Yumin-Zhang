### **Updates (Oct 9th-Oct 13th)：**

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


### **Next Steps (Oct 14th-Oct 20th)：**

* Understand, clean, and import the other two tables (skuinfo, trnsact) into PostgreSQL
*	Explore data and the table relationship and do some EDA

---

### **Updates (Oct 14th-Oct 20th)：**
* Completed cleaning the trnsact table for uploading purposes
    * Changed column names based on the column description
    * Removed duplicate rows to avoid duplicates in primary keys
    * Removed the rows whose FK cannot be matched to the tables of PK
* Finished cleaning the skuinfo table for uploading purposes 
    * Removed final three columns due to their data being incomplete
    * Removed the rows whose FK cannot be matched to the tables of PK

[So far, we imported all raw tables into Postgre]

* Cleaned the strinfo table by replacing an invalid value in the CITY column with NA 
* Corrected data type and FK, PK for all tables


### **Next Steps (Oct 21st-Oct 27th)：**:

* Feature selection, focusing on removing variables of unknown significance
* Querying out the subset of trnsact dataset to reduces the amount of data
* Update cleaned strinfo table to postgreSQL

---

### **Updates (Oct 21st-Oct 27th)：**:
* Completed input table, including defining primary keys and foreign keys, reordering columns to better align with column definitions
* Possible business problem (think about)
    * **Sales Forecasting**: Use historical sales data (SKU, SALEDATE, QUANTITY) to build a time series model. This might help businesses optimize inventory management and reduce overstock or understock situations
    * **Type of Transaction Prediction**: Use historical sales data to build a logistic regression to predict if the product will be returned (R) or not
    * **Product Clustering**: Grouping similar products together based on shared characteristics, features, or attributes. This can be useful for developing an effective marketing strategy

### **Next Steps (Oct 28th-Nov 3rd)**:

* Define the business question and corresponding machine learning question through data examination
* Feature selection, focusing on removing variables of unknown significance




