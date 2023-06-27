# SQL-Weather-Observation-Station-8

# Challenge:
- Query the list of CITY names from STATION which have vowels (i.e., a, e, i, o, and u) as both their first and last characters. Your result cannot contain duplicates.

- The STATION table is described as follows:

![n1e5uock jot](https://github.com/MarcvWaes/SQL-Weather-Observation-Station-3/assets/120553175/93033af8-77bd-460d-bf7b-fce39386b9e6)

- Where LAT_N is the northern latitude and LONG_W is the western longitude.

# Solution:
- SELECT DISTINCT CITY
- FROM STATION
- WHERE LOWER(SUBSTRING(CITY, 1, 1)) IN ('a', 'e', 'i', 'o', 'u')
  AND LOWER(SUBSTRING(CITY, -1)) IN ('a', 'e', 'i', 'o', 'u');

- By applying the 'LOWER' function, the case-sensitivity issue is being handled.
- The 'SUBSTRING' function is being used to extract the first and last characters of the 'CITY' name. 
 
# Output:
- Upperco
- Aguanga
- East China
- East Irvine
- Amo
- Eleele
- Oconee
- Amazonia
- Aliso Viejo
- Andersonville
- .....
