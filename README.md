# 1. Data Overview and Cleaning
# Key Characteristics:

Dataset Size: The dataset contains 8,784 records (rows) and 8 features (columns).
Features: The dataset includes the following columns:
* Date/Time (object): The timestamp of the recorded weather data.
* Temp_C (float64): The temperature in degrees Celsius.
* Dew Point Temp_C (float64): The dew point temperature in degrees Celsius.
* Rel Hum_% (int64): The relative humidity as a percentage.
* Wind Speed_km/h (int64): The wind speed in kilometers per hour.
* Visibility_km (float64): The visibility distance in kilometers.
* Press_kPa (float64): The atmospheric pressure in kilopascals.
* Weather (object): The recorded weather conditions.

# Missing or Null Values:

There are no missing or null values in the dataset. All columns have 8,784 non-null entries. Since there are no missing values, no imputation or removal is necessary.

# Duplicate Records:

The dataset contains no duplicate records, as confirmed by the df.duplicated().sum() result showing 0 duplicates.
# 2. Statistical Summary
Numerical Features Summary:
The dataset consists of both integer and float data types, which are summarized statistically as follows:

Temperature (Temp_C):

Mean: 8.80°C
Standard Deviation: 11.69°C
Minimum: -23.3°C
Maximum: 33.0°C
Median (50th Percentile): 9.3°C

Dew Point Temperature (Dew Point Temp_C):

Mean: 2.56°C
Standard Deviation: 10.88°C
Minimum: -28.5°C
Maximum: 24.4°C
Median (50th Percentile): 3.3°C

Relative Humidity (Rel Hum_%):

Mean: 67.43%
Standard Deviation: 16.92%
Minimum: 18%
Maximum: 100%
Median (50th Percentile): 68%

Wind Speed (Wind Speed_km/h):

Mean: 14.95 km/h
Standard Deviation: 8.69 km/h
Minimum: 0 km/h
Maximum: 83 km/h
Median (50th Percentile): 13 km/h

Visibility (Visibility_km):

Mean: 27.66 km
Standard Deviation: 12.62 km
Minimum: 0.2 km
Maximum: 48.3 km
Median (50th Percentile): 25.0 km

Pressure (Press_kPa):

Mean: 101.05 kPa
Standard Deviation: 0.84 kPa
Minimum: 97.52 kPa
Maximum: 103.65 kPa
Median (50th Percentile): 101.07 kPa

# Outlier Detection:

Temperature (Temp_C):

The minimum temperature (-23.3°C) and maximum temperature (33.0°C) are significant deviations from the mean, indicating potential outliers.
Dew Point Temperature (Dew Point Temp_C):

The minimum (-28.5°C) and maximum (24.4°C) values for dew point temperature could be considered outliers due to their deviation from the mean.
Wind Speed (Wind Speed_km/h):

The maximum wind speed of 83 km/h stands out as a potential outlier, given the mean wind speed is 14.95 km/h.
Visibility (Visibility_km):

The minimum visibility of 0.2 km could indicate an outlier due to extreme weather conditions (e.g., heavy fog).
This statistical summary provides an initial understanding of the weather dataset, highlighting the central tendency and dispersion of key weather parameters. Outlier detection is crucial for identifying unusual weather events or data recording errors that may need further investigation.
