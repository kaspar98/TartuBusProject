**Project M7: TARTU-BUS-ANALYSIS**

**Project for "Introduction to Data Science" course (2019).**

**Repository files:**
* varem.csv - original data about all the occasions when a bus departed over 10s earlier
* hiljem.csv - original data about all the occasions when a bus departed over 3min later
* DataPreparation.ipynb - data preparation file in which: the encoding of the data is changed to UTF-8; the data is combined into a single large file; formats of "estimated_departure_time" and "deviation" are repaired; fields "id", "route_long_name", "user_id", "stop_code" are deleted; rows with too deviation larger than 15min are deleted; trips with old IDs are deleted (there was an ID change in the middle of september); visual check of column values is done; several new values columns are added ("wd" - dayofweek, "route_direction_id" - identifier for route direction, "total_stops" - total amount of stops on trip).
* RoutesAnalysisByTrips.ipynb - all the graphs displayed on the poster are done here; data exploration and search for problematic trips.
* GraafikudLVle.ipynb - graphs about probability of late and early departures for each route.
* M7_report.pdf - homework 10 report.
* M7_poster.pdf - poster about project findings.
* liinide_info.csv - information about departure amounts for all lines.
* nimetused.csv - used codenames and their corresponding route directions.
* Drafts folder - contains additional .ipynb files with done data exploration.


**Project information:**

Tartu launched new inner city bus routes in 01.07.2019 [1]. Our project analyses whether the new timetables need changing or not.

Dataset 1 (56.4 MB): data from 01.09.2019-18.10.2019 with all the bus stops where the bus departed over 3 min later than supposed to. Data includes 260K rows with route numbers, dates, stop names, departure time deviations, pseudonymised bus driver names (private dataset from Tartu City Government)

Dataset 2 (24.3 MB): data from 01.09.2019-18.10.2019 with all the bus stops where the bus departed over 10 sec earlier than supposed to. Similar to dataset 1, but with 125K rows (private dataset from Tartu City Government)

Goal 1: Our main goal is to figure out do any of the new bus route timetables need changing because buses constantly arrive too early/late to some stops (find problematic bus stops).

Goal 2:  Find any interesting trends or patterns from the data that could have some practical use.

TEAM:
Kairit Peekman
Kaspar Valk
Mikk-Kaspar Tammi

Links:
[1] https://tartu.ee/et/liinivork#Liinid-alates-1.-juulist
[2] https://docs.google.com/presentation/d/1swsJMQpWBC8agwqxQSXBqnQM6WNcBkjdC-MCsscuEfw/edit#slide=id.g70b2e3acc7_6_5
