# Exploring-Weather-Trends
#### Step 1: Extract the Data
The first thing I needed to do to begin exploring weather trends was to extract my global
and local temperature data. To extract the data, I used SQL to retrieve data from three lists provided: city_list, city_data and global_data. Before I extracted data from city_data, I needed to know which city provided in the list was closest to me. To do that, I needed to look at city_list first. I used the query, “SELECT * FROM city_list” and found that it listed cities across the globe, so I needed to narrow it down. Since I live in the United States, I narrowed the data to only provide cities within the US. So I did, “SELECT * FROM city_list WHERE country = ‘United States’”. This made it much easier to find my city which ended up being Chicago. With this information, I was able to retrieve my local data. I typed: “SELECT * FROM city_data WHERE city = ‘Chicago’”, and found everything I needed, so I exported it to a .CSV file. Next, I needed global data, which was much easier to retrieve. All I had to type was, “SELECT * FROM global_data” so I exported that to .CSV too. I had everything I needed, so I decided to start step two.
#### Step 2: Create Line Charts
Now that I had all the data I needed, I exported it to a spreadsheet application. The next step is to create a visualization of my data, but I need to find the moving average first in order for my graph to look smoother. I decided to use a ten year moving average. To calculate, I found the first tenth year in the table, made another column and typed in “=AVERAGE(“. I did this to both my tables. I had the data I needed, So I created my graph:


  <img width="500" alt="Screen Shot 2022-05-09 at 9 46 16 PM" src="https://user-images.githubusercontent.com/69525188/167532661-3f764ef1-bbff-4e7b-9de1-f8323f10f7ae.png">

 
#### Step 3: Make Observations
I noticed a few trends after making my graph:
1. First, I found that my local temperature is consistently 2° higher than the global temperature which was surprising.
2. The global temperature fluctuated between 7° and 9°quite noticeably between the years 1750s and 1780s, while local remained at a consistent incline from 9° to 10° through that period.
3. Directly after that, from the years 1800s to 1820s both temperatures followed a similar trend as their temperature decreased 1° rapidly within ten years to a sharp increase of 1° a few years later.
4. Both the local and global temperatures show that average running temperatures have increased through the years(1750s-2010s). I added a trend line to showcase that. This could be from several factors like population increase, factories polluting the air and global warming.
