# HPEs\_2001\_2023_xwei_v1.0
### Paul Voit, 2024-09-6, University of Potsdam
### contact: voit@uni-potsdam.de

The catalog contains heavy precipitation events (HPEs) derived from the [RADKLIM dataset](https://opendata.dwd.de/climate_environment/CDC/grids_germany/hourly/radolan/reproc/2017_002/netCDF/)
The events are selected on the basis of an xWEI (cross-scale weather extremity index) exceedance of 10 [-] for a 3km x 3km x 3 h cube. this equals approximately an event wih rainfall exceeding the return period of ten years on one duration. Pixels that exceeded this threshold were then clustered using a voxelization method, clustering all cells within a 10 km distance.
For a detailed description of the method refer to [Voit & Heistermann, 2024](https://nhess.copernicus.org/articles/24/2147/2024/)

The catalog contains xWEI and WEI values calculated with the classical weighing of the area (area is weighed using the radius of a circle with equal size, see [Müller & Kaspar, 2014](https://doi.org/10.5194/nhess-14-473-2014) and the modified version using the natural logarithm of the area (see [Voit & Heistermann, 2022](https://doi.org/10.5194/nhess-22-2791-2022)).

## Field description

### id
Unique identifier for the event.

### xwei
xWEI of the event based on the classical calculation.

### wei
WEI of the event based on the classical calculation.

### max_dur
Duration [h] (temporal scale) at which the event was most extreme according to the WEI.

### max_area
Spatial scale [km²] at which the event was most extreme accoring to WEI.

### start_time
Starting time of event. Format: YearMonthDayHourMinute

### end_time
Starting time of event. Format: YearMonthDayHourMinute

### lat_centroid
Latitude of the centroid of the event.

### lon_centroid
Longitude of the centroid of the event.

### x_pixel_centroid
X-coordinate of the events centroid in the RADKLIM grid.

### y_pixel_centroid
Y-coordinate of the events centroid in the RADKLIM grid.

### bbox_xmin
X-coordinate of the lower x_value of the bounding box (RADKLIM coordinates)

### bbox_xmax
X-coordinate of the upper x_value of the bounding box (RADKLIM coordinates)

### bbox_ymin
Y-coordinate of the lower y_value of the bounding box (RADKLIM coordinates)

### bbox_ymax
Y-coordinate of the upper y_value of the bounding box (RADKLIM coordinates)

### bbox_zmin
Z-coordinate of the lower z_value of the bounding box (RADKLIM coordinates). Z-Axis is "time".

### bbox_zmax
Z-coordinate of the upper z_value of the bounding box (RADKLIM coordinates)  Z-Axis is "time".


### xwei_ln
xWEI of the event based on modified weighing of the area (ln(A)).

### wei_ln
WEI of the event based on modified weighing of the area (ln(A)).

### max_dur_ln
Duration (temporal scale) at which the event was most extreme according to the WEI_ln.

### max_area_ln
Spatial scale at which the event was most extreme accoring to WEI_ln.

### x_cum_rain_max
X-coordinate (RADKLIM) of the pixel with the most cumulated rainfall during the event.

### y_cum_rain_max
Y-coordinate (RADKLIM) of the pixel with the most cumulated rainfall during the event.

### lon_cum_rain_max
Longitude of the pixel with most cumulated rainfall during the event.

### lat_cum_rain_max
Latitude of the pixel with most cumulated rainfall during the event.

### x_1h_rain_max
X-coordinate (RADKLIM) of the pixel with the highest 1h rainfall during the event.

### y_1h_rain_max
Y-coordinate (RADKLIM) of the pixel with the highest 1h rainfall during the event.

### lon_1h_rain_max
Longitude of the pixel with the highest 1h rainfall during the event.

### lat_1h_rain_max
Latitude of the pixel with the highest 1h rainfall during the event.

### max_cum_rain_mm
Maximum cumulated rainfall [mm] that occurred in one pixel during the event.

### max_1h_rain_mm
Maximum 1h rainfall [mm] that occurred in one pixel during the event.

### landkreis_centroid
Landkreis where the centroid of the event was. nan describes location outside of Germany

### landkreis_1h_rain_max
Landkreis where the maximum 1h rainfall in one pixel. nan describes location outside of Germany
occurred.

### landkreis_cum_rain_max
Landkreis where the maximum cumulated rainfall in one pixel occurred. nan describes location outside of Germany


References:

Müller, M. and Kaspar, M.: Event-adjusted evaluation of weather and climate extremes, Nat. Hazards Earth Syst. Sci., 14, 473–483, (https://doi.org/10.5194/nhess-14-473-2014, 2014)[https://doi.org/10.5194/nhess-14-473-2014].
 
Voit, P. and Heistermann, M.: A new index to quantify the extremeness of precipitation across scales, Nat. Hazards Earth Syst. Sci., 22, 2791–2805, [https://doi.org/10.5194/nhess-22-2791-2022](https://doi.org/10.5194/nhess-22-2791-2022), 2022.

Voit, P. and Heistermann, M.: A downward-counterfactual analysis of flash floods in Germany, Nat. Hazards Earth Syst. Sci., 24, 2147–2164, (https://doi.org/10.5194/nhess-24-2147-2024, 2024)[https://doi.org/10.5194/nhess-24-2147-2024].




