_Respond to writing prompts here..._
1.	Find at least two web mapping examples that allow for user analysis. For each example provide: 1) a link to the web map and 2) a description of the user analysis
* This first link is for yelp, burgers near me. The user can interact with the map and analyze what is closest to them and where to go. https://www.yelp.com/search?find_desc=burgers%20near%20me&l=a%3A37.7759529%2C-122.49576649999997%2C25
* This census map allows you to analyze different counties and their migration flow between different years. https://flowsmapper.geo.census.gov/map.html

2.	Give an example of static data you might include on a web map. How is your example different from dynamic data?
*	If I ever wanted to map the movement of a species around areas of pollution like a refinery. Static data would include the point source pollution locations while the movement of the species would definitely be changing over time. You can interact with the static data through popups but the data does not move over time or as you interact with the map.
3.	Under what circumstances might you want to do some data prep in desktop GIS before incorporating data into your web map? Give an example of the type of data that might apply here.
*	Cleaning data up is a very important factor in data analysis and visualization. Being able to sort data through queries and eliminate nulls and duplicates. You can also create shapefiles very easily in arcmap that are transferable through mapbox studio. For example, My partner and I needed to clean up our 311 encampment calls to eliminate null values and duplicates that were useless in the dataset and only took up space. 
4.	What are some data characteristics that can impact rendering speed? How might you address these issues?
*	As mentioned before, duplicates in a dataset can severely impact your rendering speed especially with large datasets. Eliminating inadequate data values or duplicates can mean the difference between a 200MB dataset and a 150MB. The efficiency of your interactions and ability to show the desired conclusions is also important. Having powerful interactions rather than lots of useless tools is essential. 
5.	What is turf.js? Give an example of how you could apply a turf operation to a web map.
*	It is an open-source javascript library that helps with spatial analysis. It is helpful in creating GEOJSON data and useful as a client-side tool. You can use turf.js for accessibility purposes and proximity analysis (closest distances from a POI).
1.	Describe where the centroids variable comes from. How is it possible for you to reference this variable when you didn't declare it?
*	A centroid variable comes from the js file that was given to us. It is a global variable that can be accessed by any document within the folder in my computer. We also scripted a link to the data as a source.
2.	Why might you want to create the 'centroids-selected' layer after you've created the 'centroids' layer?
*	Creating the centroids-selected layer after the centroids layer is important because one, the centroids cant be selected if there isn’t a layer for them. And two because we don’t want to select them all, just the ones within the radius.
3.	Should you set the marker's lngLat and add it to the map? Why or why not?
*	You shouldn’t set its lngLat because it is an event (e) when the user’s click. We need its lngLat to be wherever the user wants it, not in one spot.
4.	How did you know which arguments to pass to the pip() function?
*	When putting the arguments into the pip() function, I knew I needed data for the selected points so I used Centroids and the searchRadius because those are the ones we wanted selected.

