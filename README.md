# XPath-and-XQuery
Assignment performed as part of CSE 532 Theory of Database Systems.

Homework 5: XML Queries
There are three XML documents: purchaseorders.xml, products.xml and customerinfo.xml.
These documents are also available in DB2 sample database as purchaserorder(porder), product(description), customer(info). 

You will write XML queries with Oxygen XML or DB2. 
(Please use XPath/XQuery builder view in Oxygen to edit and run the queries, otherwise you may run into a sequence error.)

Query 1. XPath (6 points). 
a. Using customerinfo.xml, write an XPath query to return the name(s) of customers who live in the city "Toronto" and have an assistant. Return names as text only. 

b. Using purchaserorder.xml, write an XPath query to return other items in an unshipped purchase order placed on "2006-02-18", which contains an item with partid "100-100-01".   

Query 2. XQuery (4 points): Write an XQuery to return the total cost (total quantities from multiple orders multiplied by the price) for each unique product (represented by partid or pid) in all purchase orders, sorted by partid.  
The result format should look like:
<totalcost partid="100-100-01">139.86</totalcost>
<totalcost partid="XXXXXXXXX">YYYYY</totalcost>
...

(Hint: You may want to group by partid using purchaseorders.xml and find the price for each product using products.xml. )
