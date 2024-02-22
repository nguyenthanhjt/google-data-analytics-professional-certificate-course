# Upload the Warehouse Dataset to BigQuery

In preparation for learning about COUNT and COUNT DISTINCT in SQL, you need to upload the Warehouse Orders dataset to BigQuery. Follow these steps to upload the data.

## Upload the Data

To begin, download the two .csv files from the attachments below:

- [warehouse-orders---orders.csv](./resouces/warehouse-orders---orders.csv)
- [warehouse-orders---warehouse.csv](./resouces/warehouse-orders---warehouse.csv)

1. **Open BigQuery Console:**
   Log in to your BigQuery account and select the project for data upload.

2. **Create Dataset:**
   In the Explorer pane, click the Actions icon (three vertical dots) and choose Create dataset.

   ![Screenshot of the Explorer pane with Actions icon](#)

3. **Configure Dataset:**
   Set the Dataset ID to "warehouse_orders," choose Multi-region as the Location type, and select US as the region. Leave the Advanced options as default.

   ![Screenshot of the Create dataset pane](#)

4. **Create Dataset:**
   Click the CREATE DATASET button to add the dataset to your project.

5. **Select Dataset:**
   In the Explorer, choose the `warehouse_orders` dataset to view the dataset info window.

   ![Screenshot of the warehouse_orders dataset info window](#)

6. **Create Table - Orders:**
   Click the + CREATE TABLE button to open the Create table pane.

   ![Screenshot of the Create table window](#)

7. **Upload Orders Data:**
   - Choose Upload from the Create table from dropdown.
   - Select the Warehouse Orders - Orders.csv file.
   - Set Table to "orders."
   - Check Auto detect under Schema.
   - Click CREATE TABLE.

   ![Screenshot of creating the orders table](#)

8. **Verify Table Creation:**
   Verify that the orders table is listed under the `warehouse_orders` dataset in your project.

   ![Screenshot of the orders table listed under warehouse_orders](#)

9. **Create Table - Warehouse:**
   Again, click the + CREATE TABLE button to open the Create table pane.

   ![Screenshot of the Create table window](#)

10. **Upload Warehouse Data:**
    - Choose Upload from the Create table from dropdown.
    - Select the Warehouse Orders - Warehouse.csv file.
    - Set Table to "warehouse."
    - Check Auto detect under Schema.
    - Click CREATE TABLE.

    ![Screenshot of creating the warehouse table](#)

11. **Verify Table Creation:**
    Verify that the warehouse table is listed under the `warehouse_orders` dataset in your project.

    ![Screenshot of the warehouse table listed under warehouse_orders](#)

12. **Preview Data - Orders:**
    - Select the orders table and preview the first 50 rows.

    ![Screenshot of data preview for orders table](#)

13. **Preview Data - Warehouse:**
    - Select the warehouse table and preview 10 rows.

    ![Screenshot of data preview for warehouse table](#)

If both data previews match, you are ready to proceed to the [COUNT and COUNT DISTINCT](./s8_pq_activity_count-n-count-distinct.md) activity.
