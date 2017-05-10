# blended learning projects for J-term

Interactive tools built with HTML, CSS, JS, Jquery, and Carto for students in J-term

## blended learning project #1

Layers:
- Campus Outline
- Campus Paths
- Trees
- Public Art
- Parking Lots
- Smith Buildings
- Mill River*

Layers can be modified with the options on the right sidebar, such as change in color, opacity, and line/marker width. 

*Layer is static.

## blended learning project #2

Layers:
- Campus Outline*
- Campus Paths*
- Trees*
- Public Art*
- Parking Lots*
- Smith Buildings*
- Mill River*
- DBH Trees

Layers can be modified with the options on the right sidebar, such as change in color, and size. 

*Layer is static.

## blended learning project 3

Layers:
- basemap
- metro_boston_tracts (displaying median home value)
- metro_boston_tracts (displaying conserved space per person)

*Layer is static.

## Blended Learning: Attribute App and Erase rr

Attribute App:
The attributes app allows users to filter the Chicopee municipal parcels dataset to the zoning and/or total acre specification of their choosing. Once users first select the parameter they want to display (zoning or total_acre) from the drop-down menu, the options that are available to them correspond to the list of possible values for the selected field. For example, the zoning parameter has the options: Ind, Split, Res, BusA, BusB while the total_acre parameter has different math symbols with a text box for entering number values. Users also have the ability to add a second criterion for filtering the parcels by clicking the plus-sign button on the right. This will instantiate the visibility of the second row where they can select another parameter through a similar process. These two selections are related by a logical operator (AND or OR), which will either show only the parcels that meet both requirements (aka AND) or those that meet at least one of the requirements (aka OR). When the Update Map button is clicked, the formatted SQL expression will query the Carto API to display the correct information entered.f

Erase App:
This application is meant to demonstrate how the erase command works in ArcGIS. When the window is loaded, the appropriate datasets (bus lines and grocery stores) are added to the map. Users are able to select one of those layers as the input feature and then the other as the erase feature. When they click Update Map, the overlaying portion is taken out of the input feature to display that layer with ‘erased’ regions. This is accomplished by querying a new SQL statement to the Carto API when that button is clicked. ST_Difference is used to take the difference between two geometries and the result is then transformed back into a readable the_geom_webmercator format for display purposes. The respective CSS styles and colors for each dataset are kept whenever this change is made. The user can click Reset to return the map to its original state.
