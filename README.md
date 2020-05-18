# ARINC424_Converter

## What is this:
This is a test project write in Python.

With this script, you can input any ARINC424 format master file, convert every line (132-characters) into Flight Simulator Plugin's specified format, so u can fly with your own tailored data.

## Plugins currently supported:

+ FSLabs ( \*.rom )   
    *Availability: D/DB/EA/EP/ER/PA/PC/PD/PE/PF/PG/PI/PN/TC (Fully functional)*

+ Jeehell (addtional.txt)  
    *Availability: D/DB/EA/EP/PA/PC/PD/PE/PF/PG/PN (Currently no plan for ER)*

+ Majectic (nd.db3)  
    *Availability: D/DB/EA/PA/PC/PG (Currently no plan for ER and PD/PE/PF)*

## Pre-requirement:
+ A dataset that comply with ARINC424 format. (version 18 is recommended)
    - A full baseline data is required when you want to output a complete data set.
    - Tailored dataset is required if you want to insert data onto file(s) produced by [Navigraph FMS Data][Navigraph] or [Aerosoft NavDataPro][NDP].
    - [FAACIFP18][FAACIFP] might work, but with no guarantee.

## Limitations:
+ Jeehell's ER, MJC's ER/PD/PE/PF needs data outside of tailored dataset (for fixes' id or coordinates), it will not avail when using add_tailored mode.

[FAACIFP]: https://www.faa.gov/air_traffic/flight_info/aeronav/digital_products/cifp/download/
[Navigraph]: https://www.navigraph.com/FmsData.aspx
[NDP]: https://www.aerosoft.com/en/flight-simulation/popular-products/navdatapro/
