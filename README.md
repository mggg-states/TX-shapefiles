# Texas Election Shapefile
This shapefile was obtained from the Texas Legislative Council and processed by members of the Voting Rights Data Institute (VRDI) and the Metric Geometry and Gerrymandering Group (MGGG). VRDI was a 2018 summer intensive sponsored by MGGG at Tufts and MIT, with major support from a Bose Research Grant at MIT and from the Jonathon M. Tisch College of Civic Life at Tufts.

The shapefile is currently available for download here: people.csail.mit.edu/ddeford/TX_vvtds.zip.

## Sources
Election data was downloaded from the Texas Legislative Council’s Texas Redistricting website (https://tlc.texas.gov/redist/data/data.html). In addition to the voting tabulation district shapefile and election data CSV files, shapefiles for state senate districts (PlanS172) and state house districts (PlanH407) were also downloaded. A 115th U.S. Congressional district shapefile was obtained from the Census (https://www.census.gov/cgi-bin/geo/shapefiles/index.php). All demographic information was compiled by the Texas Legislative Council using 2010 Census data.

## Processing
The shapefile topology was checked and minor corrections made using the check_shapefile_connectivity.py script (available in https://github.com/gerrymandr/Preprocessing). Roundoff (also available in https://github.com/gerrymandr/Preprocessing) was used to assign voting tabulation districts with U.S. congressional, state senate, and state house districts.

## Metadata
* `CNTYVTD`: VTD unique identifier
* `VTD`: VTD name
* `WHITE`: 2010 White population
* `OTHER`: 2010 Other race population
* `HISPANIC`: 2010 Hispanic population
* `TOTPOP`: 2010 Total population
* `VAP`: 2010 Total voting age population
* `BLACK`: 2010 Black population
* `BLKHISP`: 2010 Black hispanic population
* `WVAP`: 2010 White voting age population
* `HISPVAP`: 2010 Hispanic voting age population
* `BHVAP`: 2010 Black hispanic voting age population
* `BVAP`: 2010 Black voting age population
* `OTHVAP`: 2010 Other race voting age population
* `COUNTY`: County name
* `FIPS`: County FIPS code
* `PRES12R`: Number of votes for 2012 Republican presidential candidate
* `PRES12D`: Number of votes for 2012 Democratic presidential candidate
* `SEN12R`: Number of votes for 2012 Republican senate candidate
* `SEN12D`: Number of votes for 2012 Democratic senate candidate
* `TOTVR12`: Number of registered voters in 2012 general election
* `TOTTO12`: Number of ballots cast in 2012 general election
* `SEN14R`: Number of votes for 2014 Republican senate candidate
* `SEN14D`: Number of votes for 2014 Democratic senate candidate
* `GOV14R`: Number of votes for 2014 Republican gubernatorial candidate
* `GOV14D`: Number of votes for 2014 Democratic gubernatorial candidate
* `TOTVR14`: Number of registered voters in 2014 general election
* `TOTTO14`: Number of ballots cast in 2014 general election
* `PRES16D`: Number of votes for 2016 Democratic presidential candidate 
* `PRES16R`: Number of votes for 2016 Republican presidential candidate
* `TOTVR16`: Number of registered voters in 2016 general election
* TOTTO16`: Number of ballots cast in 2016 general election
* `USCD`: U.S. Congressional District ID
* `SEND`: Texas State Senate District ID
* `HD`: Texas State House District ID
* `AREA`: Area of vtd in square kilometers
* `PERIM`: Perimeter of vtd in kilometers

## Projection
This shapefile uses a NAD83/Texas State Mapping System projection (EPSG: 3081).

## Rating
We give this shapefile an A rating. All data was obtained from the state government and was processed by MGGG staff.
