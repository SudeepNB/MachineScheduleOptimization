## Running Project ##
```
python processOrder.py ./data/order.txt
```
This will load data from `order.txt` into program

## Feeding Data
There are two files inside data folder:
1. `products.txt`  
This file is equivalen to `enum` type. It lists different produt types.
The product types provides details for ProductName,Setuptime,unitProductionTime,index (Identifier). Available product types are:
ProductName,Setuptime,unitProductionTime,index
Knife,2,5,0
Spoon,3,4,1
Fork,4,8,2
2. `order.txt`  
This file contains order data.It provides the details for production order. Each proudction order is composed of OrderID,ProductID,Quantity,Deadline(in days),workindex (Identifier). AVailable example production order is:
OrderID,ProductID,Quantity,Deadline(in days),workindex
0,0,20,30,0 -Order0 with 20 Knife and deadline of 30 days
0,1,40,30,1 -Order0 with 20 Spoons and deadline of 30 days
0,2,25,30,2 -Odere0 with 25 Forks and deadline of 30 days
3,1,40,60,3 -Order 3
3,2,25,60,4 -Oder 3
2,0,20,70,5
2,1,40,70,6
1,1,20,80,7
1,2,25,80,8

## Change Planning Duration ##
By default, system takes maximum value of `deadline` from orders. You can set inside `solve()` method.

## Output ##
![Output](images/output.png)

