<h3 align="center">
  <img src="assets/nopanic.png" width="300">
</h3>

# Nopanic.io : A COVID-19 Website

A [website](https://notocovid19.herokuapp.com)  that provides contextual information to users on a web map in order to help contain the COVID-19 pandemic. Developed during [MariHacks 2020]('https://marihacks.com') and won 1st Place Overall.

Check out the Devpost [here.](https://devpost.com/software/nopanic-io)

## About

> Amidst the ongoing COVID19 outbreak, we felt a tool was needed to provide quality and fact-based - but also contextual - information in order to help mitigate the fear factor associated with such events. We wanted to offer this solution in a dashboard-type web application, all the while making it visually appealing and staying far from the bright reds and blacks, which are usually more fear-inducing than calming.
 
## What it does
> Nopanic.io offers many features. First of all, the user is able to see the different COVID19 outbreaks around the world for the present, the past, and even 7 days in the future using a machine learning model to predict the future number of cases. Although getting the big picture is always useful, we wanted to provide the user with a way to know if they have to adapt their lifestyle depending on their region's situation. Thus, by entering their location in the search bar, the user is able to see the number of cases in their region and, based on this number, is given safety guidelines and useful hotlines. For example, if the number of cases in an area is under 100, the user is told to proceed normally but to adopt good sanitary discipline. However, if the number of cases exceeds 1,000, the user better avoid using public transit and stay at home until the outbreak calms down.

## How we built it
> We extracted our data from the John Hopkins University public COVID19 open-source dataset made available on Github using pandas. We then transformed this dataset into daily sub-sections and exported them into .geojson files in order to be able to visualize them on Google Maps. This transformed data was then uploaded to a Google Cloud Storage Bucket. At the same time, we also built a machine learning model using linear regression, predicting the potential number of infected victims within the next week across all regions of the world. The frontend was built using the Flask python framework, which loaded a map after sending a request to the Google Maps API. The styling and utilities that are on the screen have all been made using scratch CSS, HTML and Javascript. Finally, Matplotlib was used to visualize the increase in the number of people infected across the years. 

## What's next for nopanic.io
> We have a few more features in the pipeline for nopanic.io. For example, we would like the resources and safety guidelines to be in sync with those offered by local authorities. We also envision adding some more graphing and prediction tools in order for users to monitor the outbreak while staying informed of the steps to follow.



## Authors

**Steven Gong** - [**LinkedIn**](https://www.linkedin.com/in/gong-steven/) - [**Github**](https://github.com/gongsta)

and **Lucas Azar** - [**LinkedIn**](https://www.linkedin.com/in/lucas-azar-a36a9a169/?originalSubdomain=ca) - [**Github**](https://github.com/lucas-azar)





