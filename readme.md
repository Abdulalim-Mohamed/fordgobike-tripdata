# Bike Share Analysis with Ford GoBike Data 
## by Abdulalim Mohamed 

[Ford GoBike](https://www.fordgobike.com/) is a bike share system located in the Bay Area, more specifically in San Francisco, East Bay, and San Jose. With 7,000 bikes distributed across those 3 regions, customers have the feasibility to unlock bikes from one station and return to any other station in the system, making them ideal for one-way trips. The bikes are available for use 24 hours/day, 7 days/week, 365 days/year and riders have access to all bikes in the network when they become a member through a monthly or yearly subscription or purchase a single ride or 24-hour pass.

## Dataset

This project used the Ford GoBike's trip data available in their [website](https://www.fordgobike.com/system-data).

I extracted trip data for the whole year of 2018 and compiled them together into 1 dataframe. Originally the compiled data contained 1,863,721 rows and 16 columns, but after cleaning the data, I ended up with the same number of rows, but only 11 columns.

- Trip Duration (seconds)
- Start Time and Date
- End Time and Date
- Start Station ID
- Start Station Name
- End Station ID
- End Station Name
- Bike ID
- User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)
- Member Year of Birth
- Member Gender

## Prerequisites

Before running the codes, you will need to install these:

- Anaconda
- Python (Minimum 3.7)
- Pandas
- Numpy
- Matplotlib
- Seaborn

## Python Notebook and Scripts

gobike_exploration.ipynb - Main project file, a IPython Notebook that contains the analysis for the project.
gobike_slide_deck.ipynb - This IPython Notebook contains starter cells to help organize the slide deck deliverable.

## Summary of Findings

In 2019, the average trip duration that the users took was around 10 minutes.

89.2% of the total trips were taken by Subscribers, which are members of the GoBike program.

Also, the age group with the most trips was between 30-35 years old.

The Customers users (casual users) usually took more time in their rides than Subscribers.

In Female , the age range of 10-20 has the longest trip duration. The longest trip duration in male belongs to the 60-70 age group. Weekdays: it implies customers probably includes tourists because most trips happen in the weekend. On the other hand, subscribers imply commuters because most trips happen in the weekdays.
## Key Insights for Presentation

For the presentation, I display the influence of variables in question (season of year, user type, user age and gender) on the Users' GoBike trip duration. I start by introducing the duration variable and followed by the main variable in question, season.

Afterwards, I introduce each of the relationship one by one. To start, I use the bar plots of duration and season to show that Summer season does have the longest trip duration. Then, I do violin plots of duration and user type. I'm only looking at
the trip duration of less than 60 minutes here, to focus the analysis. The other two variables, age and gender, are covered afterwards, using bar plots. I've made sure to use different color for each age group to make sure it is clear that they're different between bars.