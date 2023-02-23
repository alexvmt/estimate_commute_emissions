# Estimate commute emissions

In order for organizations of all kinds to become more climate-friendly, it is inevitable to measure their respective emissions.
Only then they can set clear and measurable goals and identify areas where they can achieve the largest emission reductions.

In the services sector, for example, the majority of organizational emissions typically stem from a handful of sources, such as:
- fleet of vehicles
- heating
- electricity
- purchasing goods and services
- business travel

Data on the emissions from these sources tend to be rather easily collected (e. g. bills, orders etc.).

But for another important source of emissions it seems to be much harder to get the required data: the emissions related to employees' commute.
More precisely, to compute an organization's yearly commute emissions one needs three key pieces of information:
1. mode of commute for each employee (e. g. foot/bike, public transport, car)
2. oneway distance between home and office for each employee
3. office days for each employee

One option that comes to mind quickly is to simply ask employees to provide these data.
But considering data privacy (i. e. the protection of personal data in particular) it is advised against to directly ask employees for such information.
Another more secure option would be to engage an external party to create a survey, collect the data and only report back aggregated data. This is time-consuming and costs money of course.

A simpler way is to estimate commute emissions based on a couple of organization-specific inputs and some general commute data (for Germany).
All an organization needs to provide are 4 pieces of information to get a rough estimate of their employees' commute emissions:
1. public transport share
2. car share
3. average weekly office days
4. number of employees

These 4 pieces of information should be easily collected by talking to a couple colleagues or the HR department.

Here's what an example for an organization with 500 employees for 2022 could look like:
- foot/bike share: 25% (based on the other 2 shares)
- public transport share: 40%
- car share: 35%

![yearly emissions by mode](yearly_emissions_by_mode.png 'yearly emissions by mode')

![mode and emission shares](mode_and_emission_shares.png 'mode and emission shares')

Only 35% of all employees commute by car but are responsible for 75% of commute emissions
whereas 40% of employees use public transport and are responsible for only 20% of commute emissions.
Independent of the exact numbers, the key message is:
Commuting by car is emitting much more emissions than using public transport or coming to the office by foot/bike.
See [this](https://github.com/alexvmt/estimate_commute_emissions/blob/main/estimate_commute_emissions.ipynb) notebook for more details.

Of course the resulting estimates are just that: estimates. But they allow a first quick insight into an organizations commute emissions.
Nevertheless, it might be necessary to assess commute emissions more accurately depending on an organizations goals and obligations.



## Backlog

- shift public transport and car distances distributions to account for different underlying behaviors
- add histogram that compares public transport and car distances distributions
- add widget to set inputs more conveniently
- allow users to input actual custom car distances
- add option to randomly assign weekly office days from 1 to 5
- create script to be run from the command line
- create Python package
- create interactive web app



## References and resources

- https://ecocockpit.de/
- https://www.destatis.de/DE/Themen/Arbeit/Arbeitsmarkt/Erwerbstaetigkeit/Tabellen/pendler1.html
- https://ghgprotocol.org/sites/default/files/standards_supporting/Chapter7.pdf