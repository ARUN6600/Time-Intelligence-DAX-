# Time-Intelligence-DAX-


New Measures 

1. Total_sales = SUM(data[salesamount])

2. Current_MTD_1 = TotalMTD([Total_sales],datesMTD(data[date])

3. Current_QTD_1 = TotalQTD([Total_sales],datesQTD(data[date])

4. Current_YTD_1 = TotalYTD([Total_sales],datesYTD(data[date])

5. Previous_MTD = Calculate([Total_sales],previousmonth(datesMTD(data[date])))

6. Previous_QTD = Calculate([Total_sales],previousquarter(datesQTD(data[date])))

7. Previous_YTD = Calculate([Total_sales],previousyear(datesYTD(data[date])))

8. MOM Growth = Divide([Current_MTD_1],[Previous_MTD])-1

9. QOQ Growth = Divide([Current_QTD_1],[Previous_QTD])-1

10. YOY Growth = Divide([Current_YTD_1],[Previous_YTD])-1

 
