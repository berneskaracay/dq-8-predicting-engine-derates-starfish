### Big G Express - Project to Predict Truck Engine Derates

- A truck's Engine Control Module (ECM) will derate the truck's engine when a problem occurs.   
- A partial derate reduces the engine power 25% and is denoted in Cummins engine diagnostics by an SPN of 1569 and an FMI of 31.

- A full derate limits the trucks speed to 5 mph and is denoted by an SPN of 5246 and an FMI of 0. A full derate is a severe condition that requires a wrecker to tow the truck in for serviced. The resulting cost is minimally $4000 plus lost productivity for the vehicle.

Can we understand precursor events in order to intervene before a full derate ocurs? From the customer:
<blockquote>Some of the causes are obvious, (low DEF tank limit), but many of them are not – we’re looking for the non-obvious reasons so that we may be able to establish a pattern ahead of time so that we can do preventative maintenance and keep the failure from happening.  The earlier we can catch these cases, the better. </blockquote>

#### Datasets
- `J1939Faults.csv` - 4 years of fault events (just over a million rows) for Big G's fleet.
- `VehicleDiagnosticOnboardData.csv` - diagnostic data transmitted from trucks (approximately 11.7 million rows).
- `Service Fault Codes_1_0_0_167.xlsx` - Cummins service fault codes; provides a guide to understanding fault code combinations for Cummins engines (which are the majority in our dataset).


