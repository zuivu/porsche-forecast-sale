# important changes

### df_internal update values until 21 
df_internal = test.iloc[:, :21]
df_internal.head()

### same for external values
df_external = test.iloc[:, 21:]
df_external.head()


## other important updates
- mean by month functionality added
- interpolation functionality added
- correct value extraction added. (row 50 to 255)
- fixes in differentiating between variables and target values. And between internal and external data


# roadmap for feature engineering

fixing the last values:
-[] leads (null or mean by month?, linear interpolation)
-[] premises (null, mean by month?, linear interpolation)
-[X] quotas (mean per month)
-[] sales_stock_monthly__vehiclegroup01 (very easy to compute with our new function)

What we need after that:
- getting the (or some) important values from the external data. A list would be great, With this, we can compute the missing values here.
- 