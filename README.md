# python-api-challenge

Code used to understand Folium:
https://towardsdatascience.com/creating-a-simple-map-with-folium-and-python-4c083abfff94
https://www.analyticsvidhya.com/blog/2020/06/guide-geospatial-analysis-folium-python/
and a friend of mine(thanks besant!)

These site gave me a basic rundown on how to properly implement folium to map my hotels. We did not go over mapping in class, so I used an outside rouserce that showed various ways to map, and decided to pick Folium since it looked very clean. 

AskBCS helped me immensely in Step4. 
   # Add filter and bias parameters with the current city's latitude and longitude to the params dictionary
    params["filter"] = f"circle:{lng},{lat},{radius}"
    params["bias"] = f"proximity:{lng},{lat}"
  and 
  # Grab the first hotel from the results and store the name in the hotel_df DataFrame
  try:
        hotel_df.loc[index, "Hotel Name"] = name_address["features"][0]["properties"]["name"]
    except (KeyError, IndexError):
        # If no hotel is found, set the hotel name as "No hotel found".
        hotel_df.loc[index, "Hotel Name"] = "No hotel found"
T got through with the help of ask BCS. 

