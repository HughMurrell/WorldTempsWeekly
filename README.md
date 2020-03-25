# WorldTempsWeekly

## Temperature Interpolation with Julia

In this repository we present two Julia notebooks

### `TempDataClean`

This notebook gives some idea on how the data sets from NOAA were cleaned
in order to generate the latest recorded average monthly temperatures for
weather stations around the globe.

It is not possible to run this notebook as is because the input data from
NOAA is too large storage on github repositories


### `TempInterp`

This notebook reads the cleaned version of NOAA monthly temperature data from weather stations
around the world and then iterpolates weekly temperatures for any point on the globe
from the nearest neighbor in the cleaned data set.

### Data Sets

`data_clean.csv` cleaned NOAA average monthly temperatures for stations on the globe.

`airports.csv` list of airports around the globe with their geo-coordinates

`airports_temp_augmented.csv` same as `airports` data but augmented by average weekly temperatures
obtained by running `TempInterp` notebook


### Animation

Below is a 52 frame animation of average temperatures for airports around the world.

![alt text](https://github.com/HughMurrell/WorldTempsWeekly/blob/master/anim_world_temp.gif "World Airports temperature animation")

This animation can be generated using the `TempInterp` notebook.

