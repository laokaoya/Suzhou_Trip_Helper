# Suzhou_Travel_Guide v1

👋 Thank you for watching and reviewing my newest work —— Tourists！

👀 Tourists aims to provide travelers with customized travel itineraries, including attractions, prices, nearby hotels, and restaurants. Travelers only need to select a few simple options to receive a personalized travel route. We hope it will meet and exceed your expectations!

⚡ Data: Our data is sourced from Weibo, a popular social platform in China where people can share their daily activities.

1. We first crawled the check-in data and corresponding user data from Weibo in the Suzhou area (in the millions), and tracked users who have posted on Weibo in Suzhou to obtain their global check-in data (in the tens of millions) (due to confidentiality requirements, the source data is not publicly disclosed here).
2. We used MySQL to extract information on attractions, restaurants, hotels, stations, and other points of interest, then aggregated and cleaned the data, all of which is stored in the data directory.


🌱 Model：
1. Statistical Analysis, Spatial Clustering
2. PyQt5 + Folium model
3. Map Visualization



😄 Results：
1. After running the program, a window pops up where users can select their travel preferences on the left side. The right side displays a clustered map of all the attractions.

![image](https://github.com/laokaoya/Tourists/assets/140779724/2c982f76-b07a-42cf-8d7a-046a6f437210)

2. Once selections are made, the map on the right shows the recommended travel route. It can also display daily routes and nearby hotels and restaurants based on the number of days for the trip.

![image](https://github.com/laokaoya/Tourists/assets/140779724/15ada159-43b0-49a7-b45b-1b3d26292876)


💞️ We hope our work can effectively help tourists get a better travel experience.

# Suzhou_Travel_Guide v2    (update 2024.9)
## Why we make version II?
- In the previous version, we were only able to obtain rough attraction information from the Weibo database. In Version II, after gathering various attractions and locations through the database, we aim to use web scraping from travel websites to acquire more detailed information.

- We are abandoning the original rating-based recommendation system and shifting towards a model that learns the relationship between tourists' travel routes and personalized features within the database. This enhances generalization capabilities, making it easier to expand the app to a broader scope in future versions.

- In Version I, restaurant recommendations were solely based on distance, which is unrealistic in practice. Therefore, in the new version, we plan to allow visitors to select their preferred types of cuisine, and we will comprehensively recommend the most suitable restaurants based on menus and reviews obtained from the web.

- The new version aims to implement multilingual and personalized text interaction. Additionally, user input will no longer be limited to preset options; we aim to allow users to describe their personalized needs in natural language.

## Project introduction
- We primarily used SQL to build the database and perform related queries, Python for the main part of the development, and the PyQt5 framework to implement the user interface, with OpenStreetMap as the selected map.

- We utilized the large model algorithm framework from Crew AI, leveraging multiple agents and OpenAI's English language model to enhance the precision and personalization of the recommendation algorithm. LINK：https://github.com/joaomdmoura/CrewAI/wiki 

- We established five agents to handle five tasks, which are: ① Collecting attraction information ② Collecting restaurant information ③ Planning daily itineraries ④ Visualizing the map ⑤ Adding map elements and improving layout. These tasks were connected through a sequential process to achieve the final map visualization results.





