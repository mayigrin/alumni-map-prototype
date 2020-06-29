# alumni-map-prototype
This repo contains a prototype for the MIT Muses Alumni/Member Map! To see the final product, go to [https://mitmuses.github.io/alumniMap](https://mitmuses.github.io/alumniMap)


## What this code does
Reads content from a Google Sheets spreadsheet that is auto-populated by a Google Form, and converts that content into an interactive map where each location that exists in the Sheet will be represented by a bubble on the map, and the people living in that location will appear in a popup over that bubble when it's moused over. Their name, class year, and location will also be displayed in a list below the map. Additionally, if someone fills out the Google Form again, the code will use the more recent entry in the sheet to avoid displaying one person in two different locations. If someone fills out the form saying they're not in the US, they will not appear in the map, but they will still be included in the list below.


## Resources Used
Here are some of the resources I used for this project:

- **Datamaps ([https://github.com/markmarkoh/datamaps](https://github.com/markmarkoh/datamaps)):** used as the backbone for the interactive map
- **Google Sheets Reader ([https://github.com/bpk68/g-sheets-api](https://github.com/bpk68/g-sheets-api)):** used (with slight modifications) to read the Google Sheets data
- **OpenCage Geocoder ([https://opencagedata.com/api](https://opencagedata.com/api)):** used to convert location names into latitude and longitude coordinates
