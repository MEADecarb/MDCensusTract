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

[CC0](https://creativecommons.org/public-domain/cc0/)

### Privacy Statement for the "Census Tract Finder" Application

#### Data Usage and Collection

- **Purpose of Data Collection**: The "Census Tract Finder" application is designed to provide users with information on census tracts based on the address they input. The data provided by users is used solely for the purpose of fetching relevant information from external sources.
- **Type of Data Collected**: The application collects the street, city, and state information as entered by the user. This information is necessary to perform the census tract lookup and provide accurate results.
- **External Data Sources**: The application retrieves data from external sources such as the US Census API, HB550 data, and school data repositories. The user's address information is used to fetch relevant data from these sources.

#### User Privacy and Data Storage

- **No Persistent Data Storage**: Our application does not store any user data persistently. Once the user session ends, all input data and results are discarded.
- **Disabling Usage Statistics**: In alignment with our commitment to user privacy, we have disabled the gathering of usage statistics in our application. This means no data regarding user interactions with the app is collected or analyzed.
- **No Cookies or Tracking**: The application does not use cookies or any form of tracking mechanisms to collect data about users.

#### User Consent and Data Usage

- **Consent**: By using the "Census Tract Finder" application, users consent to the temporary processing of their input data (street, city, state) for the sole purpose of obtaining census tract information.
- **Data Sharing**: No user data is shared with third parties. All data processing occurs within the scope of the application and is solely for the intended purpose as stated.

#### Data Security and Access

- **Security Measures**: While the application does not store user data persistently, it does implement standard security measures to protect the data during the user's session.
- **User Access**: Users have full control over the data they input and can choose to clear or modify their data at any time during their session.

