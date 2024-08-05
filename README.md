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

4. Identified the value of statistical concept called **Variability Pooling**, in this application. This smoothens the fluctuations in usage quantities of individual warehouses, if consumed altogether in a single warehouse. Through this, consolidated orders generate inventory holding cost savings. Created **Power Query** transformations to analyze consolidated orders
   ![image](https://github.com/user-attachments/assets/80abf8b5-99bd-47b4-b51e-f40d180ba40c)

5. Utlized **Lead Time** data from Procurement in **SAP Business Objects** to analyze Lead time variability and delays, therfore identifying actual lead time for the items. This is merged with the Usage_Variation Table.
   ![image](https://github.com/user-attachments/assets/9ec56f99-db69-4380-a7de-506d07a8e523)

6. The data model used for the report is as follows:
   ![image](https://github.com/user-attachments/assets/2fedb761-61f9-4cbe-a188-1840bb72115f)

   **RESULT**
1. The time savings obtained on consolidating the orders is visualized by the below report:
   ![image](https://github.com/user-attachments/assets/afee819f-ffd4-42f4-a752-ca62946c4a08)

2. The Inventory holding cost savings obtained on consolidating the orders is reported in three sections:
   **Section 1**: Safety stock Analysis illustrating the effect of **Variability Pooling** in smoothening the fluctuations in demand if we adopt combined usage (Without considering Lead time variability). Thus safety stock in centralized warehouse is lesser than sum of individual safety stocks among warehouses. 
   ![image](https://github.com/user-attachments/assets/31ae8662-c5ee-40ee-aa53-29c2699523df)

   **Section 2:** Safety Stock analysis just by considering lead time variability into picture.
   ![image](https://github.com/user-attachments/assets/93b95cd7-cb1b-4268-8f07-1aca56753506)

   **Section 3:** Total Safety Stock analysis considering lead time variability and demand variability. This illustrates the approximate savings in working capital if orders are consolidated
   ![image](https://github.com/user-attachments/assets/796a2c79-f807-4254-8726-a5d3872b0572)

   

   
   
   



      
   

