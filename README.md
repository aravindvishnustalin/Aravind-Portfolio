Biogen Supply Chain Analytics Project:-

**SITUATION** : Two warehouses RM1,DM1 orders materials independently for use. In some instances, there are delivery delays to one of the warehouses and so, orders delivered to the other warehouse needs to be shared. This causes shortage issues

**TASK**: Evaluate if consolidating the orders of both warehouses into one order, generates cost savings and avoids shortage issues

**ACTION**: 

1.	Utilized **SAP Business Objects** and **Oracle EBS** to extract and export the past 7 year-usage data of the required cleaning materials and warehouses(RM1, DM1) where they were used
   ![image](https://github.com/user-attachments/assets/0ff97814-de6b-4045-b462-d8936c00e7ae)

2. Investigated and identified that 3 hours of inspection time can be saved by consolidating the orders into one order. The Data transformations are performed in **Power Query** to obtain total inspection time savings per item.
   ![image](https://github.com/user-attachments/assets/5405f5bf-ebe7-456d-a568-cc994f5ba36f)


3. Two consumption patterns are analyzed using **MS Power BI** as follows: (1) Consumption pattern if orders are not consolidated (2) Consumption pattern if the orders are consolidated. 
   ![image](https://github.com/user-attachments/assets/28132378-48de-4ae9-aabe-3889e7857927)

4. Identified the value of statistical concept called **Variability Pooling**, in this application. Through this, consolidated orders generate inventory holding cost savings. Created **Power Query** transformations to analyze consolidated orders
   ![image](https://github.com/user-attachments/assets/80abf8b5-99bd-47b4-b51e-f40d180ba40c)

5. Utlized **Lead Time** data from Procurement in **SAP Business Objects** to analyze Lead time variability and delays, therfore identifying actual lead time for the items. This is merged with the Usage_Variation Table.
   ![image](https://github.com/user-attachments/assets/9ec56f99-db69-4380-a7de-506d07a8e523)

6. The data model used for the report is as follows:
   ![image](https://github.com/user-attachments/assets/2fedb761-61f9-4cbe-a188-1840bb72115f)

   **RESULT**
   



      
   

