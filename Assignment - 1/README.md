We have recorded data when the car took full circles in the parking lot. There are two circles, one of those should be processed. 

The recorded data can be downloaded from the following link: 

20240628 (Links to an external site.) 

GPS data is given in the CSV file. The lateral (lat) and longitudinal (lon) coordinates can be read from the corresponding columns.  

 

The task is to automatically and robustly segment the points corresponding to one of the turning circles and then to estimate the radius of the circle. 

 

Conversion of GPS lat/lon coordinates to spatial locations: 

x = R * cos(lat) * cos(lon) 
y = R * cos(lat) * sin(lon) 
z = R *sin(lat) 

Where R=6.371.000m (radius of Earth) 

Remark that the altitude is static, therefore it is not included in the formulas. 
