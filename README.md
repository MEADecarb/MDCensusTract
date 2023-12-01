# MDCensusTract:  Census Tract Finder Web App

This is a simple web application to find the census tract for an address and display relevant information related to Maryland House Bill 550 as well as associated schools.

## Features

- Enter any address (street, city, state) in the US  
- Uses Census Geocoding API to find census tract, block, block group for address
- Checks if census tract is listed in Maryland HB550 bill data  
- Displays key HB550 information if tract is listed
- Finds and shows schools associated with the census tract
- Built with Streamlit for the web framework

## Data Sources

The app uses the following data sources:  

- [Census Geocoding API](https://geocoding.geo.census.gov/geocoder/Geocoding_Services_API.pdf) - address lookup
- [HB550 tract data](https://github.com/MEADecarb/MDCensusTract/blob/main/HB550.json)  
- [School geo data](https://github.com/MEADecarb/MDCensusTract/blob/main/Schools_tracts.geojson)  

## Usage  

The app is currently designed to run as a Streamlit web app.  

To run locally:  

```
pip install streamlit pandas requests  
streamlit run app.py
```

The app can also be adapted to run on public cloud platforms like Heroku.  

## Customization

The core address lookup functionality can be reused and integrated into other applications.  

The HB550 and school data can be switched out to support other state policy and education scenarios.

## Further Development  

Potential enhancements:

- Improve error handling and validation
- Support batch address lookup  
- Containerize app with Docker
- Add user accounts and data persistence  

## License  

MIT
