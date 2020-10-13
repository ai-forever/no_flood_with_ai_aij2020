# Datasets description



1. ### /hydro/

   Complete archive of observation data at hydrological stations of the Russian Federal Service for Hydrometeorology and Environmental Monitoring network for the period from 1984 to 2018. Contains data on water levels, flow rates, water temperature, observation of the water surface (formation of freeze-up, opening).

- **{hydrological station number}_daily.csv**
   The files contain daily water level values at hydrological posts:

  - 'Дата' - date of measurements

  - 'Уровень средний' - average water level per day (cm.)

  - 'Уровень миним.' - minimum water level per day (cm.)

  - 'Уровень максим.' – maximum water level per day (cm.)

  - 'Темпр. средняя' - average water temperature per day (°C)

  - {many gaps}

  - 'KCBO' - water body status code. More in file '/Пояснения/гидрология 1985-2018.rtf'

- **{hydrological station number}_ice.csv** 

  Periodic values (once every 5 days) of snow height and ice thickness at the hydrological station

  * 'Дата' - measurement date

  * 'Толщина льда' - ice thickness
  * 'Высота снега' - snow height
  * 'Место измер.' - ice measurement site code. More in file '/Пояснения/гидрология 1985-2018.rtf'

- **{hydrological station number}_disch_d.csv**

  Average daily water consumption

  - 'Дата' - measurement date
  - 'Расход воды' - average daily water consumption (m3/с)

- **{hydrological station number}_disch_m.csv** 

  Monthly extremes of water consumption

  *  'Месяц.год' - month.year

  *  'Расход.минимал' - minimum consumption per month (m3/с)

  * 'День 1-ый' - the first day when the minimum flow was observed

  * 'День посл.' - the last day when the minimum flow was observed

  * 'Число случ.' - the number of times when the minimum flow was observed

  * 'Расход максимал.' - maximum consumption per month (м3/с)

  * 'День 1-ый' - the first day when the maximum flow was observed

  * 'День посл.' - the last day when maximum flow was observed

  * 'Число случ.' - the number of cases when the maximum flow rate was observed

    

2. ### /hydro_2019-2020

- **new_data_all.csv**

  File with data only about water levels for the period 01-01-1984 - 01-10-2020. It contains not only archived data, but also updated data from 2018 to the present.

  - 'time' - measurement date
  - 'max_level' - maximum level for the day
  - 'identifier' - hydrological station number

- **new_data_target.csv** 

  ​	A subset of the **new_data_all.csv** file for target hydrological posts

  

3. ### /meteo/

   Archive data of observations at the meteorological station of the Russian Federal Service for Hydrometeorology and Environmental Monitoring network from 1985 to 2018

* **{weather station number}.csv**

  * 'station_name' Station name
  * 'station_id' Station ID
  * 'visibility_distance' Horizontal visibility range
  * 'visibility_distance_quality' Quality mark
  * 'wind_direction' Wind direction
  * 'wind_direction_quality' Quality mark
  * 'wind_speed_avg' Average wind speed
  * 'wind_speed_avg_quality' Quality mark
  * 'wind_speed_sign' Presence of sign ">"
  * 'wind_speed_max' Maximum wind speed
  * 'wind_speed_max_quality' Quality mark
  * 'wind_speed_max_sign' Presence of sign ">"
  * 'precipitation_amount' Amount of precipitation for the period between periods
  * 'precipitation_amount_quality' Quality mark
  * 'temperature_ground' Soil surface temperature at time
  * 'temperature_ground_quality' Quality mark
  * 'temperature_air' Air temperature on dry term
  * 'temperature_air_quality' Quality mark
  * 'humidity' Relative humidity at time
  * 'humidity_quality' Quality attribute
  * 'time' Observation period

  More in file **/Пояснения/Метео.rtf**

  

4. ### /meteo_new

   Dataset with observation data at weather stations for the period from 01-01-1984 to 31-03-2020. Fewer stations (only those included in the World Meteorological Organization network) than in the past, but more fields and coverage

* **{weather station number}.csv**  
  * stationNumber The synoptic index of the World Meteorological Organization station
  * year (GMT)
  * month (GMT)
  * day (GMT)
  * time (GMT)
  * localYear Source year (local)
  * localMonth Source month (local)
  * localDay Source day (local)
  * localTimePeriod Source time
  * timePeriodNum Period number in days according to standard winter time (PDZV)
  * localTime Local time
  * tz Time zone number
  * startMeteoDay Beginning of the meteorological day according to PDZV
  * horizontalVisibility Horizontal visibility
  * horizontalVisibilityQuality Quality attribute
  * horizontalVisibilitySign Sign of the presence of the ">"
  * cloudCoverTotal Total amount of clouds
  * cloudCoverTotalQuality Quality mark
  * pastWeather Weather between dates
  * pastWeatherQuality Quality mark
  * presentWeather Weather at time of observation
  * presentWeatherQuality Quality attribute
  * windDirection Wind direction
  * windDirectionQuality Quality mark
  * windSpeed Average wind speed
  * windSpeedQuality Quality mark
  * windSpeedSign Sign of the presence of the sign ">"
  * maximumWindGustSpeed Maximum wind speed
  * maximumWindGustSpeedQuality Quality mark
  * maximumWindGustSpeedSign Sign of the presence of the ">"
  * totalAccumulatedPrecipitation The amount of precipitation for the period between periods
  * totalAccumulatedPrecipitationQuality Quality attribute
  * soilTemperature Soil surface temperature
  * soilTemperatureQuality Quality mark
  * groundMinimumTemperature Minimum soil surface temperature
  * groundMinimumTemperatureQuality Quality mark
  * airTemperature Dry bulb temperature
  * airTemperatureQuality Quality mark
  * minimumTemperatureAtHeightAndOverPeriodSpecified Minimum air temperature between periods
  * minimumTemperatureAtHeightAndOverPeriodSpecifiedQuality Quality attribute
  * maximumTemperatureOverPeriodSpecified Maximum air temperature between periods
  * maximumTemperatureOverPeriodSpecifiedQuality Quality mark
  * relativeHumidity Relative air humidity
  * relativeHumidityQuality Quality attribute
  * vapourPressure Water vapor saturation deficiency
  * vapourPressureQuality Quality mark
  * dewpointTemperature Dew point temperature
  * dewpointTemperatureQuality Quality mark
  * pressure Atmospheric pressure at station level
  * pressureQuality Quality mark
  * pressureReducedToMeanSeaLevel Atmospheric pressure at sea level pressureReducedToMeanSeaLevelQuality Quality attribute
  * characteristicOfPressureTendency Characteristic of the pressure tendency characteristicOfPressureTendencyQuality Quality attribute
  * HourPressureChange3 The magnitude of the pressure trend
  * HourPressureChange3Quality Quality attribute stationId local identifier (attribute _meteo_ in [Automated accounting system for observation units] (http://asunp.meteo.ru/geoits-rest/services/asunp/geo.json))

  More details in **meteo_new/readme.pdf**



5. ### /processed_data

- asunp.pkl - a table with a description of hydrological and meteorological posts. Taken from 'http://asunp.meteo.ru/geoits-rest/services/asunp/geo.json'
- daily.pkl - a table with the linked files {station_number}_daily.csv from the /hydro folder and the columns in the corresponding formats.
- disch_d.pkl - a table with the linked files {station_number}_disch_d.csv from the /hydro folder and the columns in the corresponding formats.
- disch_m.pkl - a table with the linked files {station_number}_disch_m.csv from the /hydro folder and the columns in the corresponding formats.
- ice.pkl - a table with the linked files {station_number}_ice.csv from the /hydro folder and the columns in the corresponding formats.
- meteo_coords.pkl - a table with numbers and coordinates of weather stations. Built on top of asunp.pkl
- s2m.pkl - tables with gauging station numbers, numbers, nearest weather stations and distances between them. Built on top of asunp.pkl
- station_coords.pkl - table with numbers and coordinates of hydrological posts. Built on top of asunp.pkl
