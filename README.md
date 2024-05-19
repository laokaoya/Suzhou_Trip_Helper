# Tourists

👋 Thank you for watching and reviewing My work —— Tourists！

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
2. Once selections are made, the map on the right shows the recommended travel route. It can also display daily routes and nearby hotels and restaurants based on the number of days for the trip.

💞️ We hope our work can effectively help tourists get a better travel experience.
