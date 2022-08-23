# Ford GoBike Data Exploration (San Francisco)
## by Ruth Jepngetich Kibor


## Dataset

> > This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area for February 2019.The data has the following columns:
- Start date and time - "start_date: start date of trip with date and time"
- Start station location - "start_station: station id of start station"
- End date and time - "end_date: end date of trip with date and time"
- End station location - "end_station_id: station id of end station"
- Bike number - "bike_nr: id of bicycle used"
- Membership type - "subscription_type: (should be cognizant of varying membership types)"
- age of member (of registered user) - "birth_date: birth year of user"
- gender of member (of registered user) - "gender: gender of user"

> The data is obtained from https://github.com/BetaNYC/Bike-Share-Data-Best-Practices/wiki/Bike-Share-Data-Systems 
> I used pandas to load a csv file of the data which i then exploreb by using various functions such as .info(), .describe(), and dtypes. I realised that there were several null rows in the data which I removed for easier working. I also created new columns such as age by subracting the member_birth_year from 2019. I also obtained a column 'day' which has the day of the week when the ride took place. I also removed some columns that I would not be using. 

## Summary of Findings
> A majority of bike users in San Francisco are around 20-40 years old. There are some outliers in the ages. There seems to be a 140 year old cyclist.
> The distribution of duration of ride in minutes skewed to the left.
> A majority of the riders are male,followed by females and then other.
> The day of the week with most rides is Thursday!
> Around 160,000 people did not participate in the bike share.
> Majority of the riders are subscribers. 
> The gender with the longest ride duration is the 'Other' gender, followed by 'Female' and then 'Male'.
> Plenty of people between the age of 25-75 ride their bikes for a duration of less than an hour, however, a few people in this age group also ride their bikes for more than 20 hours.
> Only subscribers are in the bikes shares.
> A large number of subscribers are male at 119,000.
> The median age of customers and subscribers is around 30 years. The customer group has an outlier of 140 years old while the subscriber has an outlier at around 120 years.
> The gender 'Other' has a young population of ridrs with a majority between 20 and 60. The outlier with 140 years of age is a female. We can also see that a lot more males ride longer durations compared to the other genders.

## Key Insights for Presentation

> My main features of consideration were: 
<ol>
    <li> Duration of the ride</li>
    <li> The member gender </li>
    <li> The user type </li> 
    <li> The user's age</li>
</ol>

> From the exploration, my key insights are: 
-  A large number of subscribers are male at 119,000.
- From this faceted scatter plot, we can clearly see that the gender 'Other' has a young population of ridrs with a majority between 20 and 60. The outlier with 140 years of age is a female. We can also see that a lot more males ride longer durations compared to the other genders.
- A majority of the riders are male,followed by females and then other.
    