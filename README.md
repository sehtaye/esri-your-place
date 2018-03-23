Your Place: 
=============
A 2018 ECCE App Challenge Entry
-------------------------------
**Team Members**

* Edward Seh-Taylor
* Jack You
* Matthew Kipp
* Yorgan Pitt

**Purpose**: To compliment the [Royal LePage](https://www.royallepage.ca/en/) website presenting housing data in the City of Toronto by determining perferred housing locations using nearby school and hospital preferential algorithms. As of the 22nd of March, the [bRoyal LePage](https://www.royallepage.ca/en/) website does not take nearby schools and hospitals into consideration. 

In particular, the app will display all Toronto houses where the user will query to slim the selection of houses down by number of bedrooms, bathrooms, price, and closeness to schools and hospitals. Clicking on found house will popup the information that was searched along with the address and a link to further inspect the house.

**Usage Instructions**:

The app is available via web browser at [kippmr.com/esri-your-house](http://www.kippmr.com/esri-your-house/) and operates on mobile and desktop devices.
Instructional video on using the app: [WE DO NOT HAVE A VIDEO YET](https://youtu.be/3iMuzuwukKc)

App Characteristics:
--------------------
Our app contains listings of homes in the City of Toronto listed for sale on the Royal LePage website worth $100,000 and $2,000,000 along with their lat/long coordinates, price, number of bathrooms/bedrooms, building type, address, and link to the actual listing. The existing Royal LePage website lacks the ability to find preferred homes for the user to purchase based on importance of closeness to schools and hospitals.

We have improved on this my using open data provided by the City of Toronto to generate overlapping maps of closeness to schools and hospitals. This was uploaded to an ESRI ArcGIS Server as a Network Analysis serice, allowing us to query the service with the user's selected filters and find the appropriate number of homes to that the user would like most from their schools and hospitals priority slider. Then we use those house points to populate a FeatureLayer from the ArcGIS JS Web API that the user can see and click on to learn more information about via a pop-up of the selected home.

Data Sources:
-------------
* [Data Source One](https://feeds.bikesharetoronto.com/stations/stations.xml)
* [Data Source  Two](http://www1.toronto.ca/wps/portal/contentonly?vgnextoid=9ecd5f9cd70bb210VgnVCM1000003dd60f89RCRD&vgnextchannel=1a66e03bb8d1e310VgnVCM10000071d60f89RCRD)
* [Data Source Three](http://www1.toronto.ca/wps/portal/contentonly?vgnextoid=71d9c7e6e34b6410VgnVCM10000071d60f89RCRD)
* [Royal LePage website listings](http://www.royallepage.ca/en/)

Limits and Assumptions:
-----------------------
* To remove any outliers, any homes listed at below $100,000 and greater than $2,000,000 were removed from our dataset. Ideally the data will contain accurate data from any price range.
* The app currently only uses listing posted by Royal LePage because other realty companies have users agree not to use their data for purposes other than viewing. In the future we would like this app to include listings by more than one realtor by partnerships.
* Homes may only be located within Toronto at the moment due to keeping the scale of the application low to ensure quick development of the proof-of-concept as well as simplify the collection of realtor listings.

Improvements:
-------------
* Finding more datasets to further refine our maps could add more filters for the user to refine their search for a new home. Such as entertainment, parks, and restaurants.
* Adding route calculations to where a home selected is from the user's workplace (that the user would enter themselves)

**Disclaimer**: *Your Place is not affiliated with any of the organisations or programs present in the app. The app was made strictly for educational purposes in conjunction with the 2018 ECCE App Challenge. This app is a prototype and all calculations are purely estimates. The app was tested on and works with Chrome and Firefox web browsers.*
