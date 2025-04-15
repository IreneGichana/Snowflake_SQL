# Snowflake_SQL
Exploring London's Travel Network
London, or as the Romans called it "Londonium"! Home to over 8.5 million residents who speak over 300 languages. While the City of London is a little over one square mile (hence its nickname "The Square Mile"), Greater London has grown to encompass 32 boroughs spanning a total area of 606 square miles!
Given the city's roads were originally designed for horse and cart, this area and population growth has required the development of an efficient public transport system! Since the year 2000, this has been through the local government body called Transport for London, or TfL, which is managed by the London Mayor's office. Their remit covers the London Underground, Overground, Docklands Light Railway (DLR), buses, trams, river services (clipper and Emirates Airline cable car), roads, and even taxis.

In this project, we will work with a slightly modified version of a dataset containing information about public transport journey volume by transport type.

## Questions of analysis
1. What are the most popular transport types?
2. Days the bus is the most busy
3. Which five months and years were the most popular for the Emirates Airline? 
4. Find the five years with the lowest volume of Underground & DLR journeys
5. Popularity of the Tram

The data has been loaded into a Snowflake database called TFL with a single table called JOURNEYS, including the following data:
### TFL.JOURNEYS

| Column | Definition | Data type |
|--------|------------|-----------|
| `MONTH`| Month in number format, e.g., `1` equals January | `INTEGER` |
| `YEAR` | Year | `INTEGER` |
| `DAYS` | Number of days in the given month | `INTEGER` |
| `REPORT_DATE` | Date that the data was reported | `DATE` |
| `JOURNEY_TYPE` | Method of transport used | `VARCHAR` |
| `JOURNEYS_MILLIONS` | Millions of journeys, measured in decimals | `FLOAT` |

## Data Analysis and Insights
### Most popular transport type
![Screenshot (2876)](https://github.com/user-attachments/assets/82dc6eb5-ab4c-44fb-aa09-ab19f29a77e0)

### Popular days by bus
![Screenshot (2878)](https://github.com/user-attachments/assets/2fcab6b4-cab9-4fe7-8209-0924368ec909)

### Emirates airline popularity
![Screenshot (2879)](https://github.com/user-attachments/assets/418c828c-4f47-4cbd-a68a-e23bc8dc9130)


### Least tube year popularity
![Screenshot (2880)](https://github.com/user-attachments/assets/02dc3220-52fa-4c41-a10d-874c6eba5d62)

### Tram popularity
![Screenshot (2882)](https://github.com/user-attachments/assets/fe2ace10-5f22-4000-b3fc-288eaf8e3718)
