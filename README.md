# HW2


#### Question1 
Using the framework presented in class create a semivariogram for the MT air quality data set. See below.

```{r}
aq <- data.frame(station =c ('Billings-Lockwood','Birney','Bozeman','Broadus','Butte',
'Flathead Valley','Frenchtown','Great Falls','Hamilton','Helena','Lewistown','Libby',
'Malta','Missoula','Seeley Lake','Sidney','Thompson Falls','West Yellowstone'),
                 pm2.5 = c(11.4, 5.2, 7.2, 5.0, 8.0, 7.6, 6.5, 8.2, 4.6, 9.3, 2.6, 7.6, 
                 2.9, 3.9, 16.0, 2.2, 8.1, 1.2),
                 lat = c(45.78218, 45.36620, 45.68379, 45.44007, 46.00240, 48.363694, 
                 47.01290, 47.49417, 46.24583, 46.6588, 47.048537, 48.38416, 48.317507, 
                 46.84222, 47.17564,  47.80342, 47.59639, 44.65703),
                 long = c( -108.51153, -106.48943, -111.05634, -105.37024, -112.50089, 
                 -114.189272, -114.22427, -111.30278, -114.15886, -112.0131, -109.455315, 
                 -115.54805,  -107.862471,  -114.01972,  -113.47623,  -104.48562,  
                 -115.32361,  -111.08958 ))              
```

##### a. (5 points)
Create a plot to visualize the air quality at the observed station locations.

##### a. (9 points)
Create and plot a semivariogram and discuss the range (or effective range), sill, and nugget implied by your figure. Please talk about them in the context of the data set (in terms of distance between sites and measurement).

##### b. (3 points)
Create a semivariogram using the function available in R. Discuss any differences between the two figrues.

##### c. (3 points)
Given the semivariogram, which covariance function would you specify and why?
