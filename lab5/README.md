# Lab 5 San Francisco Bay Traffic

## 1. Study Area + dates

I chose to request the bay from about the golden gate to the Carquinez strait for January 7th to 9th of 2023. Converting the time from UTC makes it 4pm on the 6th of January through 3:59pm on the 9th of january. I chose the bay because I liked its ferries, ships, and boats all in one place over the weekend, using each filter and I chose those dates because they covered the weekend and a weekday so I can see the difference. The data comes from AccessAIS (BOEM, NOAA, and U.S. Coast Guard): https://marinecadastre.gov/accessais/. To keep it managable I used a tight box and short window of 3 days. The csv has 500k reports from about 496 vessels which after converting to json is about 489 with 2 positions drawn.

## 2.Interpretation 

Across the vessels theres about 9-16 moving an hour at its lowest at around 3-4am and about 46 vessels on saturday at 11am, 58 on sunday at 2pm, and 66 on monday at 9am. As for the passenger boats i noticed them in stationary clusters around San Fran, Oakland, berkeley, Alameda, and Richmond docks at about 5am. Movement then starts about an hour after and peaks at 1pm during the weekend(18 vessels moving on saturday and 19 on sunday). I am guessing that because of there being more commuter service on a workday is the reason that Monday had more moving vessels than the weekend with 33 compared to the weekend's 24 vessels a day. For the cargo ships they mostly stayed still as 10 of 44 cargo ships never moved along with 2 of the 13 tankers. 

## 3.Feature Proposal

For a kayaker or small sailboat skipper that wants to cross the bay when ferry and ship traffic is light. A feature that shows how many vessels are moving each hour with the vessel type as a bar chart or something would be a good idea. The kepler.gl time playback guide (https://docs.kepler.gl/docs/user-guides/h-playback) has a time distribution display, which is a bar graph that shows how much data falls in each part of the timeline. The user could then see that traffic is lowest at 3-4am and pick to cross then during that quiet window, instead of struggling through the animation to guess.