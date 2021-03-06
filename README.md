# Coral app for GovHack Datathon 

## Back-end API development
- Using Flask as a framework as an API interface to the coordinate data displayed on the map.
- Use a lightweight development base on the back end and add features as needed
- The back-end API is connected to a Mysql database and has a certain error tolerance.
- The back-end developed a cache mechanism, because the query coordinates of the data requires algorithmic computing time, so the cache can greatly reduce the length of time the user waits for data display

## Coordinate processing back-end development
- The camera locations are not around the river, so to simulate a polluted river and make the project more meaningful, all camera locations are automatically assigned by the algorithm to a specific river location.
- The calculation is done using a matching search algorithm based on the manhattan distance.
- The use of cache mechanism greatly reduces user waiting time

## Front-end Dashboard Development
- The front-end theme framework using Wordpress for secondary development
- Use responsive pages on the front end and integrate modules such as data display, map display, video display, project monitoring, etc.

## Front-end Maps Development
We use the Google Maps platform, which uses real-time data and real-time imagery to create an immersive location experience that allows users to make more appropriate business decisions. The main advantage of Google Maps is that it allows users to embed "maps" into a website without having to build their own map server. By bringing in the Victoria River Map dataset into the map, users can clearly see the distribution of rivers in Victoria. In addition, data from individual monitors is presented as markers on the map, while the data of monitors are matched to the rivers nearest to them based on an algorithm, allowing a clear view of the waste data collected by the nearby monitors integrated on each river. The garbage data is also color-coded depending on the amount.
In addition, we also used Echarts, which is an open source visualization library implemented in JavaScript. It relies on the vector graphics library ZRender, which is both intuitive and interactive, as well as highly customizable data visualization charts. After retrieving the data from the server, the data is further formatted and processed.

## Convolution Neural Network
- Used pytorch for CNN and pretrained the data using ResNet architecture.

## Forecasting
- Used ARIMA Time Series model for Forecasting.

## Tableau 
- Tableau Dashboard is used for creating the correlation visualization between City of Melbourne suburbs and events conducted in the suburbs.

## Application Dashboard
Please navigate to http://govhack.eventplus.cc/
