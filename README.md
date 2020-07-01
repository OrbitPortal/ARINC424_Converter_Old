# ARINC424_Converter

## What is this:
This is a test project write in Python.

With this script, you can input any ARINC424 format master file, convert every line (132-characters) into Flight Simulator Plugin's specified format, so u can fly with your own tailored data.

## Plugins currently supported:

+ FSLabs ( \*.rom )   
    *Availability: AS/D/DB/EA/EP/ER/PA/PC/PD/PE/PF/PG/PI/PN/TC (Fully functional)*

+ Jeehell (addtional.txt)  
    *Availability: AS/D/DB/EA/EP/ER/PA/PC/PD/PE/PF/PG/PI/PM/PN/PT (ER requires Baseline or navrecord.dat from Navigraph/NDP)*

+ Majectic (nd.db3)  
    *Availability: D/DB/EA/ER/PA/PC/PD/PE/PF/PG/PI (Fully functional)*

+ Aerosoft (Various Files)  
    *Availability: D/PA/PG (May requires Baseline or NDB from Navigraph/NDP)*


## Pre-requirement:
+ A dataset that comply with ARINC424 format. (version 18 is recommended)
    - A full baseline data is required when you want to output a complete data set.
    - Tailored dataset is required if you want to insert data onto file(s) produced by [Navigraph FMS Data][Navigraph] or [Aerosoft NavDataPro][NDP].
    - [FAACIFP18][FAACIFP] might work, but with no guarantee.

## Limitations:
+ Jeehell's ER needs a Baseline dataset/FS NavData to process (for fixes' coordinates).
+ MJC's ER/PD/PE/PF needs a Baseline dataset/FS NavData to process (for fixes' id or coordinates).
+ Aerosoft may requires Baseline dataset/FS NavData to process (for fixes' coordinates).


[FAACIFP]: https://www.faa.gov/air_traffic/flight_info/aeronav/digital_products/cifp/download/
[Navigraph]: https://www.navigraph.com/FmsData.aspx
[NDP]: https://www.aerosoft.com/en/flight-simulation/popular-products/navdatapro/
