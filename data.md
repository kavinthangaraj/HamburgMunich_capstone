**Project Data**

The borough and neighborhood data for both cities are taken from City Population website [1] and saved as excel sheet.

[Munich data](https://www.citypopulation.de/en/germany/munchen/admin/)

The excel file contains borough and neighborhood (quarters) details for both cities with population estimates for the year 2018.

Obtained data is parsed using *pandas* library. Using *geopy* library, latitude and longitude for each neighborhood is obtained. Then the neighborhoods are separated based on respective boroughs and are plotted on city map using *folium* library.

Using the *foursquare location data* venues around each neighborhood is extracted for their name, location and type (food shops, cafes, park, etc.). Then each neighborhood is analyzed (and saved in a dataframe) for common type of venues and the category of venues are ranked based on occurrences.

With the final dataframe, the neighborhoods are clustered based on the similarity of venues. *K-means clustering from sci-kit learn library* is used for this step and final conclusions are derived from the obtained results.






**Reference:**

1 [Thomas Brinkhoff: City Population](http://www.citypopulation.de)
