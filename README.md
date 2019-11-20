# Scooter_Density
## Overview
This is the repo for a full-class project in which we analyzed the data gathered by The Metro Nashville City Planners on Scooter Operators in Nashville. After basic exploratory analysis, my team focused on the data's adherence to the guidelines for data reporting outlined in the city ordinance that governs scooter operation in Nashville.
The ordinance can be found [here](https://www.nashville.gov/Metro-Clerk/Legislative/Ordinances/Details/7d2cf076-b12c-4645-a118-b530577c5ee8/2015-2019/BL2018-1202.aspx).

Further, I also had a special role within the class as the presentation compiler. I ordered slide submissions by all teams, controlled theme, and wrote all the transitional/orientation slides.

The presentation of the class findings can be viewed [here](https://cdn2.hubspot.net/hubfs/4020755/Scooter%20Project%20Presentation.pdf)
IMAGE OF FIRST SLIDE
## Project Takeaways
This was a massive project that really tested our abilities not only as individual analysts, but at teammates as well. The data was just so large and the scope of the question so great that we really had to trust that our teammates and the other teams would do their part on their part to make the whole come together. It was also interesting for me as the presentation compiler, because I had to judiciously split my time between my contribution to my team and working to make the whole presentation come together.

## The Pitch
The Metro Nashville City Planning Department asked: What is the Ideal Scooter Density for Nashville? They were also interested in identifying data quality issues, in any insights we could present regarding current use, in suggestions we could offer for targeting specific high-need, low-income areas of the city, and any other relevant information analysis turn up.

## The Data
This dataset was very large. We had to use pickling in Python to really even create workable chunks due to the sheer size. The actual types of data reported were controlled by a city ordinance, which can be found [here](https://www.nashville.gov/Metro-Clerk/Legislative/Ordinances/Details/7d2cf076-b12c-4645-a118-b530577c5ee8/2015-2019/BL2018-1202.aspx).  

## Approach to the Problem
Analysis of the data proceeded in Python using Jupyter notebook. We also utilized some geopandas to map the location data. My basic approach was to start with a general analysis of the data. I identified the scooter companies who are currently operating ("operators"), get a general idea of the statistics of rides (how long, how many/period, where, rises/falls in use, etc. both overall and by operator).

I was really captivated by the ordinance, though. I kept noticing little things about the data. I got annoyed when I found large numbers of trips under 1 minute, for example. Those should have been cleaned out, I complained, and they *weren't*. Well, my team reasoned, the City Planner did ask about data quality issues. So then we set out to analyze and visualize the noncompliant data. For example, this is a plot showing scooter trips by duration.
IMAGE OF USET
The horizonal black line is set at 24 hours, the upper limit according to the ordinance, of reported trip durations. All the dots above it *should* have been removed from the data before it was submitted to Metro. 

We were able to come up with several ways of quantifying  noncompliance to be actionable by pointing out which operators were currently the most compliant and therefore the easiest to work with.  
IMAGE OF BAR, IMAGE OF DONUT
