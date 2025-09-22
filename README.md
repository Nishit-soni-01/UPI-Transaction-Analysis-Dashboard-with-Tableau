# UPI-Transaction-Analysis-Tableau-Dashboard

### Dashboard Link: https://public.tableau.com/views/dashboard-2_17566265495720/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Problem Statement

This project involves the creation of a dynamic, multi-page Tableau dashboard to provide a 360-degree view of UPI transaction data. The goal is to analyze overall transaction metrics, compare the performance of different banks, understand the geographical spread of transactions, and profile customer demographics and behavior. This tool enables stakeholders to identify key trends, top-performing banks, high-activity locations, and valuable customer segments.

### Steps Followed

-   **Step 1: Data Connection and Preparation**
    -   Connected to the `UPI Transactions` CSV data in Tableau.
    -   Utilized the **Data Source page** for data preparation, such as verifying data types and establishing any necessary relationships.

-   **Step 2: Calculated Fields**
    -   Created a **Calculated Field** to categorize customers into different `Age Groups` for demographic analysis. The logic used was:
    ```
    IF [CustomerAge] <= 24 THEN "A1"
    ELSEIF [CustomerAge] <= 35 THEN "A2"
    ELSE "A3" END
    ```
    -   Developed several other core calculated fields for the main KPIs, including `Total Transaction Amount`, `Total Transactions`, and `Average Transaction Amount`.

-   **Step 3: Dashboard Design and Navigation**
    -   Designed an intuitive and interactive four-dashboard story with clear navigation actions.
    -   The workbook is segmented into: a **Main Dashboard**, **Bank Wise Analysis**, **Location Wise Analysis**, and **Customer Analysis**.

-   **Step 4: Worksheet and Dashboard Creation**
    -   **Main Dashboard:** Created KPI text objects for primary metrics, a pie chart for "Transaction Status," a bar chart for "Transaction Amount by Gender," a line chart for "Month Wise Transaction," and a pie chart for "Transaction Type."
    -   **Bank Wise Analysis:** Built bar and pie charts to compare banks by transaction count and value, supplemented with a detailed text table.
    -   **Location Wise Analysis:** Used a map worksheet to show "Total Transaction Amount by Location" and a table for detailed location data.
    -   **Customer Analysis:** Designed a pie chart for "Customer by Age Group," a bar chart to identify the "Top 10 Customers," and a detailed customer information table.

-   **Step 5: Publishing**
    -   The completed dashboard was published to **Tableau Public** (or Tableau Server) to be shared with stakeholders.

---

# Dashboard Snapshot

The workbook is a multi-page dashboard that allows for a deep dive into different aspects of the UPI transaction data.
<img width="1907" height="966" alt="Screenshot 2025-09-22 205616" src="https://github.com/user-attachments/assets/029e365c-201b-4d47-9b2a-62cd9f87a159" />
<img width="1909" height="968" alt="Screenshot 2025-09-22 205605" src="https://github.com/user-attachments/assets/2cceaf51-b11c-4427-854a-dda6cb6b588a" />
<img width="1892" height="982" alt="Screenshot 2025-09-22 205543" src="https://github.com/user-attachments/assets/03fbfdb2-86d3-44f7-956b-aa9cdd064351" />
<img width="1915" height="985" alt="Screenshot 2025-09-22 205626" src="https://github.com/user-attachments/assets/833f40d4-0dde-4dde-a141-2312bab1f52f" />



---

# Insights

### [1] Overall Transaction Trends

-   **Key Metrics:** The platform processed **2.1K transactions**, amounting to a total value of **₹1.2 Crore**, with an average transaction value of **₹5.7K**.
-   **Transaction Status & Type:** The pie chart indicates a high success rate, with the majority of transactions being **Completed**. The "Transaction Type" chart highlights the most common uses of the UPI platform.
-   **Monthly Performance:** The line chart reveals the transaction trends over time, helping to identify peak months and growth patterns.

### [2] Bank Performance Analysis

-   The "Bank Wise Analysis" dashboard identifies the **top-performing banks** both in terms of total transaction volume and total transaction value. Banks like HDFC, ICICI, and SBI are key players in the ecosystem.

### [3] Geographical Insights

-   The map visualization on the "Location Wise Analysis" dashboard pinpoints the **cities and regions with the highest transaction activity**, indicating key geographical markets for digital payments.

### [4] Customer Demographics & Behavior

-   **Age & Gender:** The dashboard provides a clear breakdown of the user base by **gender** and **age group**, identifying the most active demographic segments.
-   **Top Customers:** The "Top 10 Customers" chart highlights the most frequent users of the platform, who could be targeted for loyalty programs or further engagement.
