# Menentukan Primary key table customer
SELECT CustomerID, COUNT(CustomerID)
as Total_cust
from `bi-muamalat2022.Final_Task.Customers`
GROUP BY 1
Order by 1 desc
Limit 5;

# Menentukan Primary key table order
SELECT OrderID, COUNT(OrderID) as
Totalorders FROM `bi-muamalat2022.Final_Task.Orders`
GROUP BY 1
ORDER BY 2 DESC
LIMIT 5;

# Menentukan Primary key table product
SELECT ProdNumber, COUNT(*) AS
Total_Products
FROM `Final_Task.Products`
GROUP BY ProdNumber
LIMIT 5;

# Menentukan Primary key table product_category
SELECT CategoryID, COUNT(CategoryID) as
Total_Kategori FROM
`Final_Task.ProductCategory`
GROUP BY 1
ORDER BY 2 DESC
LIMIT 5;

Query Join Antar Table
Select
o.Date as order_date,
pc.CategoryName as category_name,
pr.ProdName as product_name,
o.Quantity as order_qty,
pr.Price as product_price,
(o.Quantity*p.Price) as total_sales,
c.CustomerEmail as cust_email,
c.CustomerCity as cust_city

FROM `bi-muamalat-2022.Final_Task.Orders` od
      LEFT JOIN `bi-muamalat-2022.Final_Task.Customers` cs ON od. CustomerID = cs.CustomerID
      LEFT JOIN `bi-muamalat-2022.Final_Task.Products` pr ON pr. ProdNumber = o.ProdNumber
      LEFT JOIN `bi-muamalat-2022.Final_Task.ProductCategory` pc ON pc. CategoryID = p.Category
ORDER BY 1 ASC
