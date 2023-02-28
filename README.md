# Estimate employee commuting emissions

For organizations of all kinds to become more climate-friendly, it is inevitable to measure their respective greenhouse gas emissions.
Only then they can set clear and measurable goals and identify areas where they can achieve the largest emission reductions.

In the services sector, for example, the majority of organizational emissions typically stem from a handful of sources, such as:
- fleet of vehicles
- heating
- electricity
- purchasing goods and services
- business travel

Data on the emissions from these sources tend to be rather easily collected (e. g. bills, orders etc.).

But for another important source of emissions it seems to be much harder to get the required data:
the emissions produced by employees commuting between their homes and their worksites.
In general, to calculate an organization's annual employee commuting emissions one needs 3 key pieces of information:
1. modes of transport for each employee (e. g. foot/bike, public transport, car)
2. one-way distance between home and worksite for each employee
3. number of office days in the respective period for each employee

One option that comes to mind quickly is to simply ask employees to provide these data.
But considering data privacy (i. e. the protection of personal data in particular) it is advised against to directly ask employees for such information
- even if anonymized as there remain challenges regarding storage, security and access to just name a few.
Another more secure option would be to engage an independent external party to create a survey, collect the data and only report back aggregated data.
This is time-consuming and costs money of course.

A simpler and faster way is to estimate employee commuting emissions based on a couple of organization-specific inputs
and some general commuting data (for Germany in the present case).
All an organization needs to gather are 4 pieces of information to get a rough estimate of their employee commuting emissions for a given period:
1. public transport share (i. e. share of employees commuting mostly on public transport)
2. car share (i. e. share of employees commuting mostly by car)
3. average weekly office days (i. e. the average number of days per week people come to the office)
4. number of employees

These 4 pieces of information should be fairly easily collected by talking to a couple colleagues or the HR department.



## Example

Here's what an example for an organization with 500 employees for 2022 could look like:
- public transport share: 40%
- car share: 35%
- foot/bike share: 25% (based on the other 2 shares above)
- average weekly office days: 3

Emissions - 2022
- total: 220.72 t CO2e
- per employee: 0.44 t CO2e

![annual emissions by mode](annual_emissions_by_mode.png 'annual emissions by mode')

![mode and emission shares](mode_and_emission_shares.png 'mode and emission shares')

Only 35% of all employees commute by car but are responsible for 75% of emissions
whereas 40% of employees use public transport and are responsible for only 25% of emissions.
Independent of the exact numbers, the key message is:
Commuting by car is emitting much more emissions than using public transport or coming to the office by foot/bike.
See [this](https://github.com/alexvmt/estimate_employee_commuting_emissions/blob/main/estimate_employee_commuting_emissions.ipynb) notebook
for more details.

Of course the resulting estimates are just that: estimates. And the emissions produced from working at home are also not considered, for example.
But the presented approach allows a first quick insight into an organization's employee commuting emissions.
Nevertheless, it might be necessary to assess employee commuting emissions more accurately depending on an organizations goals and obligations.



## Backlog

- enable default setup
- add widget to set inputs more conveniently
- shift public transport and car distances distributions to account for different underlying behaviors
- add histogram that compares public transport and car distances distributions
- allow users to input actual custom car distances
- add option to randomly assign weekly office days from 1 to 5
- create script to be run from the command line
- create interactive web app
- create Python package



## References and resources

- https://ghgprotocol.org/sites/default/files/standards_supporting/Chapter7.pdf
- https://www.destatis.de/DE/Themen/Arbeit/Arbeitsmarkt/Erwerbstaetigkeit/Tabellen/pendler1.html
- https://www.destatis.de/DE/Themen/Arbeit/Arbeitsmarkt/Erwerbstaetigkeit/aktuell-erwerbstaetigkeit.html
- https://ecocockpit.de/