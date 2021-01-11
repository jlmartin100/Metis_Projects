## MTA Turnstile Traffic Analysis

### Project Description:

The prompt for the project was an email from a fictional organization, Women Tech Women Yes(WTWY), requesting data analytics support.  They wished to identify the MTA turnstiles with the highest traffic, in order to place street teams for lead generation for fundraising and a gala ticket giveaway.

### Features and Target Variables

The original dataset consisted of eleven columns of data, comprised of the audit date, station name, control area, remote unit, SCP (original turnstile), number of entries, and number of exits, as well as the MTA division, the train lines served by that turnstile, and a description column pertaining to the auditing of the turnstile entries and exits.  

Our focus here was on the **date and time** features, the combination of **control area/remote unit/individual turnstile unit**, and the **entries counts**.

Our target variables were the **turnstile entries totals and averages**, computed by station and by control area/remote unit/SCP sub unit, and calculated as daily totals, weekly averages, and week over week averages to show highest traffic days of the week.

Using these variables, we analyzed:

- the stations with the highest average weekly turnstile traffic for the date range chosen
- the highest turnstile usage per control area/unit
- the average weekly activity, plotted week over to week to visualize highest traffic days of the week
- the top five highest weekly average turnstiles for the top three highest weekly average stations

### Data Used 
**Source**:     [http://web.mta.info/developers/turnstile.html](http://web.mta.info/developers/turnstile.html).  

**Date range**: April 29, 2019 - June 3, 2019.  

We chose this date range based on the following assumptions:

- The gala would only occur in a post-COVID return to normal movement and gathering
- Data prior to 2020 would be needed in order to analyze normal traffic patterns
- Since the gala would occur in early summer, data just prior to the early summer period was desirable.

### Tools Used 
  - Pandas
  - Matplotlib
  - Seaborn
  - The map generator at [https://www.subwayridership.nyc/](https://www.subwayridership.nyc/)
  
### Possible Impacts:

In the fictional scenario given by the prompt, our analysis would support WTWY in building their e-mail leads list to maximize their fundraising, invite a broad range of gala guests, and potentially invite gala guests to their programs promoting the inclusion of women in the technology sector.
