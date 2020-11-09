# EHAM v0.1
This is a file to add EHAM (Amsterdam Schiphol Airport) to the [Endless ATC](https://steamcommunity.com/app/666610) game.

## Features
### Implemented
* Arrivals and departures at EHAM
* (Semi-)Realistic arrival- and departure paths
* Realistic airspace
* Secondary airports: EHRD
* Multiple runway configurations (currently 2)
### Planned
* Realistic airline schedules. The variety of airlines is quite limited at this time.
* Additional runway configurations
* Add EHLE secondary

## Basic operations
### Departures
### EHAM
Each departure will follow a realistic SID from the departure runways.
Departures are generally cleared to climb to FL130 after initial contact to approach.
When arrivals need to be vectored overhead the airport or away from the standard vectors, departing aircraft are kept at FL60 until clear of the conflict.

### EHRD
Departures in real life are coordinated with EHAM APP before being released.
Departures towards the south, west and south-east can usually be cleared to FL60 and then to FL130 when clear of EHAM arrivals to RIVER.
Departures towards the north should be cleared to climb to FL130 when clear of the potential arriving traffic 36R.

### Arrivals
### EHAM
Arrivals to EHAM arrive to the TMA through 3 main entry points:
* SUGOL (from the west)
* ARTIP (fron the (north)east)
* RIVER (from the south)

All arrivals are routed to SPL after the entry point in the standard vectors.
As such the arrivals from SUGOL and ARTIP are routed to SPL in the sim, arrivals from the south are initially routed to RIVER.
In real life these arrivals would be with Amsterdam Radar still as the EHRD TMA it flies over only goes up to FL55.
Arrivals via RIVER should be directed to SPL after RIVER for standard vectors.
A basic guide for vectoring including a diagram is included at the [IVAO Netherlands website](https://nl.ivao.aero/atc/vectors).

The following are basic vectoring guidelines

### South Configuration (config 1)
Aircraft are routed to SPL and descended to FL40 (Transition level based on Endless ATC parameters).
When aircraft are cleared for the initial descend timely, departures should have no problem climbing over.
Be specifically mindful of departures to IDRID or BERGI.
Then aircraft are vectored on a righthand downwind for ILS18R or lefthand downwind for ILS18C.
Aircraft landing 18R are descended to 3000ft on downwind, then 2000 ft on the base turn.
Aircraft landing 18C are descended to 3000ft on downwind and remain at 3000ft on base and until intercepted.
Ensure that the downwind leaves sufficient room for the base turn.

Alternatively, aircraft from RIVER can be given heading 020 and aircraft from SUGOL and ARTIP are flown direct towards SPY (Spijkerboor).
Then the aircraft are descended to 2000ft and 3000ft for RWY 18R and 18C respectively.
This is useful at low traffic amounts, but as traffic gets higher, the extra track miles help with separation.

### North Configuration (config 2)
Aircraft from SUGOL are vectored for runway 06 and aircraft from ARTIP for runway 36R.
Aircraft from RIVER can be vectored to either runway 06 or runway 36R depending on other traffic.

Aircraft from SUGOL are directed to SPL and down to FL40, then turned downwind heading 240.
Then descended to 3000ft on the downwind and to 2000ft on the base turn.

Aircraft from ARTIP are directed to PAM descending to FL40 and leave PAM heading 205.
Then the aircraft is descended to 3000ft on the heading of 205 and descended to 2000ft on the base turn.

Aircraft from RIVER are either vectored for a straight in ILS06 and controlled by speed to merge with traffic from SUGOL.
Aircraft from RIVER to RWY36R are put on a heading of 060 and descended to FL040, be mindful of departures from EHRD.
Then the aircraft are merged with traffic from ARTIP based on speed and intercept distance.

### EHRD
Arriving traffic from EHRD will arrive from all four cardinal directions.
Arrivals from the north and east are routed to PAM, from the west to STD and from the south directly to ROT.
Arrivals are then routed to ROT and flown either a righthand circuit for runway 06 or lefthand circuit for runway 24.
Aircraft arriving from PAM towards runway 24 are usually vectored straight in, likewise for west and south arrivals for runway 06.

Notice bugs or issues? Please open an [issue on github](https://github.com/AdamJCavanaugh/EndlessATCAirports/issues).

##Changelog
v0.1 Initial release

v0.2
* Corrected initial beacon west arrivals to EHRD
* Added EHAM_readme.md


## Credits
All coordinates and other information with respect to EHAM/EHRD where directly taken from the [eAIP](https://www.lvnl.nl/eaip/2020-10-22-AIRAC/html/index-en-GB.html).
