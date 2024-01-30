# Bis Group6

## Todo's
### Feature Engineering
- [ ] Building a month feature. Instead of 1-255 use 1 to 12


## 1. Features information 
### 1.1. Internal features (1152 in total)
For each vehicle group (64 vehicles), we have 18 features:  
1. Sales info:
    1. **sales_actuals_monthly__vehiclegroup01__orderintake**: TARGET VARIABLE
    2. sales_actuals_monthly__vehiclegroup01__retail;
    3. sales_flow_monthly__vehiclegroup01__cp8;
    4. sales_stock_monthly__vehiclegroup01__physical;
    5. sales_stock_monthly__vehiclegroup01__grossall;
    6. sales_stock_monthly__vehiclegroup01__netimporteranddealer;

2. Customer relationship:
    1. customer_vehicle_relationships__vehiclegroup01__active_cars;
    2. customer_vehicle_relationships__vehiclegroup01__terminated_cars;

3. Leading
    1. leads__vehiclegroup01__first_touch_point;
    2. leads__vehiclegroup01__won;
    3. leads__vehiclegroup01__lost;

4. Leasing:
    1. leasing_contracts__vehiclegroup01__start;
    2. leasing_contracts__vehiclegroup01__end;

5. Premises:
    1. premises__vehiclegroup01__flag_production_start
    2. premises__vehiclegroup01__flag_order_start;
    3. premises__vehiclegroup01__in_sales;
    4. premises__vehiclegroup01__in_production;

6. Quota:
    1. quota__vehiclegroup01__aq;

![Internal feature image](img\internal_feature_metadata.png)


### 1.2. Global features (1217 in total)
![External feature image](img\external_feature_metadata.png)


## 2. Questions to Porsche
- What does cp stand for? sales_flow_monthly__cp8 -> production: central point 8 (1 to 8) 8 means it is finished and at the end of the conveyer belt
- sales_stock: cars physically at the Porsche center; in Europe less countries in stock than in US or China as the transport ways are shorter over here; Chinese dealers just order cars without having customer requests; 
- sales stock: still at side, on a ship (import), at dealers- grossall: all cars in stock (produced but not retailed yet), independent of order is behind it or not; n

- What is sales_stock_monthly_netimporteranddealer 
Cars that have left the prodcution; either on importer or on dealer leevl; NET means no customer order connected to it -> customer is yet to be found

gross-all: total cars in stock; also cars that do not have an order from the customer (independent from order status)
physical: car is physically on the dealer's side, e.g. in the Porsche center



- Does physical & grossall data inclzde the netimporteranddealer?

- premises_in_sales : Local sales on Porsches own sales sides
Start of prod, start of sales -> Macan: just had start of sales, customers can now order it. Stock is prepared and now customers can order the car. End of prod: car is not produced in factory but can still be bought.
If all cars produced have been sold, than this is called end of sales.

These dates are called premises.


phd? 



