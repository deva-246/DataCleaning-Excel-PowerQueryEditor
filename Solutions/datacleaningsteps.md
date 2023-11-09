## Data cleaning and transformation steps 

1. Remove unwanted columns, which does not support our insight extraction process. The unwanted columns in the given dataset were - sno, order_id and delivery_date

2. The owner requires the sales and profit details with respect to each year, on that case we don't require the full date of order, instead we only require the year. To extract the year from the order_date,

   2.1 Duplicate the order_date to extract the year
   2.2 Select copy of order_date > split columns > by delimiter > '-' > rightmost value
   2.3 As we require the Year - it is present in the right most column

3. There are 2 columns named name and Mr/Ms/Mrs, this looks irrelevant and thus can be merged into a single column as 'full name'.

    3.1 To merge the columns, select both the columns > right click > merge columns

    3.2 Now, mention a seperator if needed, in our case mr/mrs/ms.name would do, so mention a dot as a 
        seperator

4. Now add a new column named as 'Shipping' to the exisisting table.


