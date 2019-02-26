# WFDF SOTG Raw Data Repository

In the lack of any publicly query-able repository of SOTG and game scores and related data for WFDF events, I'm dumpinfg this data in here for now as CSV files.

Eventually these should go into a neat, queryable database.

## Intended Datasets

Ideally, I would like to have following datasets in a repository:

- **Events List:** Growing list of all WFDF events and their details: Name, start- & end-date,	scope & type, surface, host country & city, website
- **Teams:** Growing list of Teams participating at WFDF events with their details: Name, country & city
- **Event Teams:** Growing list mapping the teams to the events with their details: Event, divison, seeding, result for games & SOTG
- **People:** Growing list of people (players, coaches, managers, etc.) involved with the teams with their: WFDF ID, name *(Note: this may have to sit elsewhere for confidentiality purposes)*
- **Event Rosters:** Growing list mapping the people to the event teams with their details: Team, role
- **Games:** Growing list of game results bringing together the teams with their details: Event, division, date & time, field number & type, event stage, team & opponent, goals & offence time & offence goals, time-outs & spirit time-outs, SOTG scores given per dimension *(short summary of this [full game data](http://live.wcbu2017.org/game/647-mix-can-usa))*
- **Support Enums:** All the fixed values and some mappings like: age + gender -> division and country => continent

