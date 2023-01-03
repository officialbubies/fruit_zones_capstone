# fruit_zones_capstone

Overview:
This project was inspired by the Healthy People 2030 initiatives created by the US Dpeartment of Health and Human Services and the Office of Disease Prevention and Health Promotion. 

* I am not affiliated with, or employed by either of these entities.

Main:
Many people in the United States don’t eat a healthy diet. To reduce the risk for chronic diseases and improve overall health, it is recommended to eat healthier foods like whole fruit. 

Goals:
The goal of this project is to provide regional analysis of obesity and consumption behaviors along with optimal fruit tree planting zones. By combining this data we can gain insight as to which areas and demographics would benefit most from localized fruit growth. 

After regional analysis has been done to determine high priority regions and demographics for implementing health initiatives, considering what grows where is the next thing to observe and record. 

By looking at plant hardiness zones and fruit tree varieties that can be grown in those zones, we can begin to see which varieties of fruit trees can most successfully be grown in those regions.

Using the interactive folium map we can select to view hardiness zones and areas of low income and access, as well as view a list of fruit tree types that can be grown in those regions.

Python Libraries:
    
    Webscraping and cleaning:
        - requests
        - BeatifulSoup (from bs4)
        - pandas

    Plotting:
        - shapely (geometries)
        - geopandas
        - matplotlib (pyplot)
        - folium (MarkerCluster, IFrame, Map, FeatureGroup,       
        Marker, LayerControl, Popup)
        - geoplot (crs)
        - mapclassify
        - plotly
        - json

Data Sources:

    Nutrition, Physical Activity, and Obesity - 
    https://nccd.cdc.gov/

    Fruit Trees and Affiliated Zones - 
    https://www.cumminsnursery.com/

    Educational Attainment - 
    https://www.census.gov/

    Hardiness Zones geojson - 
    https://cartographyvectors.com/

    US States geojson - 
    https://eric.clst.org/tech/usgeojson/

    US Fruit and Vegetable Consumption - 
    https://www.americashealthrankings.org/

    US State Abbreviations - 
    https://worldpopulationreview.com/states/state-abbreviations

Notebooks:

    1. cummins_scrape-v3.ipynb:

            - Script for scraping Cummins Nursery fruit tree data and saving to CSV.
    
    2. break_out.ipynb:

            - Load, clean, explore fruit tree data.
            - Load US map geodata and Hardiness Zones geodata
            - Create and transform datasets for plotting
            - Explore plotting data with:
                - matplotlib
                - plotly
                - folium
                - geoplot
            
    3. intake_freq_scrape.ipynb:

            - Script to scrape table for fruit consumption data and save to CSV.

    4. health_and_intake.ipynb:

            - Load intake CSV, explore and clean
            - Create geodataframe for visual analysis
            - Regional analysis using States geodata and barplots and choropleths (matplotlib)    
            - Load education and obesity datasets, transform, visualize using barplots.
            - Stylizing of graphs

    5. state_edu_plotly.ipynb:

            - Create geodataframe using Regional and Educational Attainment data.
            - Choropleths using Plotly
    
    


