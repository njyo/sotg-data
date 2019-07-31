# WFDF SOTG Raw Data Repository

In the lack of a publicly query-able repository of [WFDF](http://wfdf.org) game scores and [SOTG](http://www.wfdf.org/sotg/about-sotg) data, this repository provides a CSV dump of all data excavated. Eventually this data shall be in a neat, queryable database.

## Structure

In order to build a cohesive and rich data-set, following data will be collated here:

- **General data**
	- `data/Events.csv`: Growing list of WFDF events and their details
	- `data/Players.csv`: Growing list of players, that have participated in WFDF events—N/A
	- `data/Teams.csv`: Growing list of teams, that have participated in WFDF events—N/A
- **Event data**
	- `data/YYYY-Event-Games.csv`: List of all games and results from an event
	- `data/YYYY-Event-Participants.csv`: List of all teams participating at an event—N/A
	- `data/YYYY-Event-Rosters.csv`: List of all team rosters at a given event—N/A
- **Schema and structure**
	- `schema/Enums.csv`: List of all  enums used to structure the data
	- `schema/` has a sample file for each of the data sets, same as below

**Note:** Until the status of privacy protection/policy is clarified, personal information will not be uploaded.

## Schema

The listed data sets are structured as follows:

### Events
Growing list of WFDF events and their details

**Example**

| Event ID | Name | Abbreviation | Year | Scope | Type | Surface | Host | Country | Start Date | End Date | Website |
|---|---|---|---|---|---|---|---|---|---|---|---|
| `2019-WU24UC` | `World Under-24 Ultimate Championships` | `WU24UC` | `2019` | `World` |  `National` | `Grass` | `Heidelberg` | `GER` | `2019-07-13` | `2019-07-20` | `https://wu24heidelberg.com`
| `2018-EBUCC` | `European Beach Ultimate Club Championship` | `EBUCC` | `2018` | `Europe` | `Club` | `Beach` | `Castelldefels` | `ESP` | `2018-10-26` | `2018-10-28` | `https://ebucc2018.org`
| Year-Abbreviation | Event Name | Event Abbreviation | Year | World, Africa, Americas, Asia Oceania, Europe | Club, National | Beach, Grass | Host city, province | IOC host country code | ISO date | ISO date | URL |

### Players

Growing list of players, that have participated in WFDF events

**Note:** Not available; until the status of privacy protection/policy is clarified, personal information will not be uploaded. 

**Example**

| WFDF ID | Gender | Date of Birth | Nationality |
|---|---|---|---|
| `1` | `Female` | `1990-01-01` | `USA` |
|`2`| `Male` | `1989-12-31` | `JPN` | 
|WFDF id number | Female, Male | ISO date | IOC country code |

### Teams

Growing list of teams, that have participated in WFDF events

**Note:** Not available

**Example**

| Team ID | Team Name | Country | City | 
|---|---|---|---| 
| `AUS-SampleTeam` | `Sample Team` | `AUS` | `Sydney` |
| `AUS-SampleSquad` | `Sample Squad` | `AUS` | `Melbourne` |
| Country-TeamName | Team name | IOC country code | City name |

### Event: Games

List of all games and results from an event.

| Event ID | Division ID | Date | Time | Field # | Field | Stage | Game Detail | Team | Opponent | Goals | Offence Time | Offence Goals | TOs | Spirit TOs | Rules | Fouls | Fair | Pos | Comm | Total | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |---|---|---|---|---|---|---|---|---|
| `2018 WMUCC` | `M-M` | `2018-07-29` | `17:30` | `Arena` | `Showcase` | `Group` | `A2 vs A4` | `SUN` | `Quantum` | `13` | `2m 17s` | `13`| `2` | `0`| `2` |  `2` | `3` | `3` | `2` | `12`|
| `2018 WMUCC` | `M-M` | `2018-07-29` | `17:30` | `Arena` | `Showcase` | `Group` | `A4 vs A2` | `Quantum` | `Sun` | `15` | `1m 05s` | `13`| `1` | `0`| `2` |  `2` | `3` | `3` | `2` | `3`|
| Event ID | Division ID | ISO date | 24h time | Filed number | Normal, Showcase | Group, Crossover, Playoff, Placement, Finals | Free text | Team name | Teams to be scored name | Number of goals | Avg. time spent on offense | Number of goals scored when starting on offence | Number of timeouts called | Number of spirit timeouts called | 0–4 | 0–4 | 0–4 | 0–4 | 0–4 |0–20|

### Event: Participants

List of all teams participating at an event

**Note:** Not available

**Example**

| Event ID | Team ID | Age | Gender | Division | Seeding | Result |
|---|---|---|---|---|---|---|
| `2018-WUCC` | `AUS-SampleTeam` | `All` | `Women` | `A-W` | `1` | `2` |
|`2018-WUCC` | `AUS-SampleSquad` | `All` | `Mixed` | `A-X` | `5` | `1` |
| Event ID | Team ID | U17, U20, U24, A, M, GM, GGM | Men, Mixed, Women | Seeding number | Final result |

### Event: Rosters

List of all team rosters at a given event

**Note:** Not available; until the status of privacy protection/policy is clarified, personal information will not be uploaded. 

**Example**

| Event ID | Team ID | WFDF ID | Number | Player | Captain | Spirit Captain |
| `2018-WMUCC` | `AUS-SampleTeam` | `1` | `3` | YES, NO | YES, NO | YES, NO |
| `2018-WMUCC` | `AUS-SampleTeam` | `4` | `3` | YES, NO | YES, NO | YES, NO |
| Event ID | Team ID | WFDF ID | Player number | YES, NO | YES, NO | YES, NO | 
