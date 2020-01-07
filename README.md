# LOCAwap
Crabeater seal diving data

Each file contains diving data for crabeater seals along the western Antarctic Peninsula for the years 2001, 2002 and 2007 (files named accordingly)
Crabeater seals were outfitted with Sea Mammal Research Unit Satellite Relay Data Loggers (SRDL), and the data were transmitted vie the Argos satellite system
Please, contact lahuckst@gmail.com for any questions of if you plan on using these data.

File columns titles are defined as follows:
REF           A three-part code (e.g. rs3-Fred-07) : The first part identifies the batch of
              tags, the second part is the name or number of the animal, the third part is
              the year 
PTT           Argos PTT number used
CNT           The number of times that this record was received
DE_DATE       Dive end: the time at which the depth crossed the threshold on the return to the
              surface
SURF_DUR      Surface duration (seconds): the length of time following DE_DATE before the
              next dive or other event began.
DIVE_DUR      Dive duration (seconds): the length of time between the crossing of the divestart threshold on the descent and DE_DATE
MAX_DEP       The maximum dive depth recorded
D1 – D9       Intermediate depth points (metres) in the dive. For most deployments one of
              these is guaranteed to be the maximum depth (so MAX_DEP is not transmitted)
V1 – V5       Speeds (metres/second) in each section of the dive. If there is one more Vvalue than D- values then V1 is the speed up to D1, V2 between D1 and D2, etc.
              The last V- value is the speed between the last D- value and the surface.
              If there are three V- values then V1 is the speed from the surface to the D1
              point, V3 is the speed from the last depth point to the surface, and V2 is the
              speed over the remainder of the dive between D1 and the last depth point.
LAT           An approximate position for the end of the dive, interpolated along the track
LON           joining the filtered positions either side of the dive in time.
TRAVEL_R      An estimate of speed-over-ground, based only on filtered Argos locations not the turbine speed (metres/second)
HOMEDIST      Great-circle distance from the home point in the deployments table*
START_LAT     As for LAT,LON but for the start of the dive
START_LON
BOTTOM        An estimate of the ocean depth derived from the Smith and Sandwell gridded dataset (metres)
T1 – T9       The percentage of DIVE_DUR elapsed since the beginning of the dive at each of the intermediate depth points
D_SPEED       The average speed recorded in the dive (metres/second)
N_DEPTHS      The number of intermediate dive points present
N_SPEEDS      The number of intermediate speeds present
DEPTH_STR     The D1,D2,D3,… values as a comma-separated string
SPEED_STR     The V1,V2,V3,… values as a comma-separated string
PROPN_STR     The T1,T2,T3,… values as a comma-separated string
PERCENT_AREA  Used to calculate the TAD dive index (see separate explanation)
SUNALT *      replaced by the function sun_alt()
SUNRISE *     replaced by the function sun_rise()
SUNSET *      replaced by the function sun_set()
RESIDUAL
GRP_NUMBER    Shows which dives were sent in the same transmission 
