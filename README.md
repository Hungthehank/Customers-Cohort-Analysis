# Customers-Cohort-Analysis

Use Python to create a Cohort chart to analyze customer behavior (number of customers staying after the first month) and make comments.

## Dataset
![image](https://github.com/user-attachments/assets/e206c8d9-6069-4afb-abb4-3d9a13583a2b)
![image](https://github.com/user-attachments/assets/8e6a0d98-6e48-4fdc-8533-9eba48e7b8a7)

## EDA

- Select necessary colomns
  ![image](https://github.com/user-attachments/assets/b6ca3154-b6a2-4ca6-811c-3d6f81f04c07)
  
- filter 'order_status' == 'Approved' and rows are not duplicated
  ![image](https://github.com/user-attachments/assets/2c9e98bf-d22a-4531-9565-3208d9d52a85)

## Create transaction_month, cohort_month, cohort_index column

- Create transaction_month
  ![image](https://github.com/user-attachments/assets/3198096f-c169-487e-8f2e-42c797890950)
  ![image](https://github.com/user-attachments/assets/91b6dd7a-4629-4047-8fc1-686c93605b37)

- Create cohort_month (each customer's earliest month of making transaction)
  ![image](https://github.com/user-attachments/assets/80db585f-a73e-4f0f-8bb4-8fa8b2690df4)
  ![image](https://github.com/user-attachments/assets/ce21d1b1-08aa-4763-b882-ff1d0270cd1d)

- Create cohort_index (Difference between current month and first month in which transaction is made)
  ![image](https://github.com/user-attachments/assets/cd1b3558-cc7f-48ec-9205-79225d9ac6cf)
  ![image](https://github.com/user-attachments/assets/873f476b-23b0-468e-8338-d5e559dc17c9)

## Create pivot_table & plotting heatmap for retention

- Create cohort pivot_table
  ![image](https://github.com/user-attachments/assets/451f0871-8187-433c-a815-f32c09993182)
  ![image](https://github.com/user-attachments/assets/98a843e9-b1a1-4162-8ba6-eab57a3273ae)

- Calculate retention rate per month index
  ![image](https://github.com/user-attachments/assets/b4be0e70-0df8-4a97-87b4-ed09e5cd331a)
  ![image](https://github.com/user-attachments/assets/3bebd2a9-c4ff-4e3a-9767-f93dc8264edd)

- Plotting heatmap for retention table
  ![image](https://github.com/user-attachments/assets/6fca71f4-f804-4b92-853d-78563efd4c4a)
  ![image](https://github.com/user-attachments/assets/58e5158a-8329-4d55-9a3d-c2ebc6a912a3)

## Comments
- The first month to the second month decreased significantly (to about 30-35%), but the following months the number of customers remained quite stable.
- Looking closely, the number of customers using the service increased in October and November, this could be due to some promotional event that attracted more users than in the other months.
