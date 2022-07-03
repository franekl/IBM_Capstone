IBM DATA SCIENCE PROFESSIONAL CERTIFICATE

\- CAPSTONE PROJECT -

“THE BATTLE OF NEIGHBORHOODS”

FRANCISZEK LISZKA - AUGUST 2021

COPENHAGEN, DENMARK





\- OPENING A CAFÉ IN COPENHAGEN –

\1. Introduction

1.1 Background

Copenhagen (Danish: København) is the capital and most populous city of Denmark. As of

1 January 2021, the city had a population of 799,033. It forms the core of the wider urban

area of Copenhagen (population 1,336,982) and Copenhagen metropolitan area (population

2,057,142). Copenhagen is situated on the eastern coast of the island of Zealand, and it is

separated from Malmö, Sweden, by the strait of Øresund.

For a number of years, Copenhagen has ranked high in international surveys for its quality

of life. Its stable economy together with its education services and level of social safety

make it attractive for locals and visitors alike. Although it is one of the world's most

expensive cities, it is also one of the most liveable with its public transport, facilities for

cyclists and its environmental policies.

1.2 Business problem

There are coffee spots everywhere in Copenhagen, people could not survive without them.

Copenhageners simply love cafés. That is the Scandinavian “coffee culture”. Cafés are

obviously not only a place where you drink a coffee, but they are also a great place to meet

friends and chat, or even do some project, work on something. Nowadays, we’re seeing more

and more people working in the cafés, it became some sort of a trend to go to such place

with your laptop.

Now, let’s look at the business side, what if someone wanted to open a café in Copenhagen?

There’s already so many… does it even make any sense? Are there any places in the city

where such a business could potentially bring profit? Let's find some places, where it could

be feasible with minimum competition around. I am going to perform the analysis which

will help me better understand which parts of the city potentially lack cafés. I am going to

use metro stations in Copenhagen as a reference point. Metro stations are the "centers" of

the city and thir nearby areas are key places when it comes to venues like restaurants or

cafes.

1.3 Interest

Anyone who would like to open a café in the Copenhagen area may be interested in this

project. The analysis can help small businesses to determine possibly the best place to open

a café business in the capital of Denmark.





\2. Data

2.1 Data sources

•

•

•

•

Copenhagen districts data – Wikipedia [1]

Metro stations data – Wikipedia [2]

Geographical coordinates of districts/metro stations – Geocoder Python Library [3]

Venues by given districts/metro stations – Foursquare API venues method [4]

2.2 Data selection and usage

• I have used Copenhagen metro stations as reference points to analyze the

restaurants and cafés that are nearby. At first, I have performed the exact same

analysis but with the city districts data. Unfortunately, it wasn’t too accurate, and

some important parts of the city have been skipped. Therefore, I have decided to use

the metro stations and their coordinates. I have also used Python Folium library to

draw maps based on the latitude and longitude of each station.

References:

•

•

•

•

[1] Category: Districts of Copenhagen

[2] Copenhagen Metro Stations

[3] Python Geocoder Library

[4] Foursquare API





\3. Methodology

•

As I have mentioned before, I have decided to use metro stations as reference points.

In my opinion, stations are a good measure of where the city life is and so where the

restaurants, cafés and bars are. I retrieved 38 metro stations that exist in real life. I

have added 5 more, that will be opened by 2024. What is more, I have added one

that does not exist and is not in plan. The reason behind that is that there was a

small circle in a map that did not include any venues and that is because it was too

far from the stations. I do live in Copenhagen myself and so I’m convinced that this

place is essential when it comes to city life.

• I have used Foursquare API venues methods in order to get venues that are situated

nearby. That means that I have obtained every venue within the distance of 700

meters of each station.

• I have used the venues data in various ways, the main goal was to get the number of

certain venues nearby each station in order to notice the possible lack of cafés,

comparing for example with the number of restaurants nearby.





•

There are 234 unique categories, and the top 10 venue counts are listed below…first

and second place do not surprise. If you’re looking into opening a café in

Copenhagen, don’t leave yet! It’s not the end… with my analysis, I will try to help

you find a place with a minimum competition around and believe me, there are such

places… even in Copenhagen.

•

Let’s now compare the restaurant count and café count by each metro station area.





•

•

•

The bar chart shown above finally gives us an approximate idea of how the number

of restaurants compares to the number of cafés around each metro stations.

I used a heatmap for counts of restaurants in neighborhoods, using Folium library.

The white circle indicates the distance of 2km within the Copenhagen center.

The cafés are marked with red markers. This helps us understand, where we might

potentially lack a café, compared to the number of restaurants.





•

I used agglomerative clustering to cluster neighborhoods based on the count of

venue categories in each one. I decided to separate the neighborhoods into 3 clusters.





•

•

•

Cluster 1: Red (Scandinavian Restaurant, Clothing Store, Beer Bar)

Cluster 2: Purple (Café, Coffee Shop – most common venues in 12 metro stations!)

Cluster 3: Cyan (Coffee Shop, Pizza Place, Grocery Store)





\4. Results

•

From the bar chart, I have concluded that many areas have a café count that is close

to 40-50% of the restaurant count. There are also some stations (let’s say first four in

the chart), that have a relatively small percentage of coffee places compared to

restaurants. As an example - Marmorkirken station has a very percentage, that is,

only 6 cafés with 40 restaurants nearby.

•

From heat maps, I have concluded that Fredriksstaden area has a very high density

of restaurants but only a few cafes, that is a great place to look into when thinking of

opening a café.

\5. Discussion

•

•

Purple cluster metros are the ones that dominate in the number of cafés and coffee

shops. Those areas are located outside of the city center.

The red clusters are the ones located in the city center. They have a wide variety of

venues and number one, two and three dominant venues are usually restaurants,

clothing stores and bars.

\6. Conclusion

•

I have chosen Fredriksstaden area as a great place to open up a café in Copenhagen.

This area is highly populated, visited both by tourists and locals and is very close to

the actual city center.

•

Fredriksstaden area is densely populated with restaurants. It naturally should be

full of cafés, but in fact, it’s not. There are very few cafés there and I can see a huge

potential of opening up a business.






