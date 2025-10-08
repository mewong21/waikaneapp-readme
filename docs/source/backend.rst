Backend
=======

Data Files
**********

Stream Data
-----------
* :code:`Waikane_Stream_Data.json` - Waikāne stream data
* :code:`Waiahole_Stream_Data.json` - Waiāhole stream data
* :code:`Punaluu_Stream_Data.json` - Punalu'u stream data
* :code:`Stream_Trend_Data.json` - Stream trend data

Tide Data
---------
* :code:`Waikane_Tide_Data.json` - High and low tide observations for Waikāne
* :code:`Waikane_Tide_Curve.json` - Past and predicted tide levels for Waikāne
* :code:`1612480_tide_predictions.csv` - NOAA tide predictions for Mokuoloe

Flood Thresholds
---------------
* :code:`Flooding_Thresholds/Waikane_16294900_stream_flood_thresholds.csv`
* :code:`Flooding_Thresholds/Waiahole_16294100_stream_flood_thresholds.csv`
* :code:`Flooding_Thresholds/Mokuoloe-Waikane_tide_flood_thresholds.csv`
* :code:`Flooding_Thresholds/Poamoho_rain_gauge_thresholds.csv`
* :code:`Flooding_Thresholds/Waiahole_rain_gauge_thresholds.csv`

Data Analysis
*************
* :code:`Waikane_Flood_Visuals.ipynb` - Jupyter notebook for data analysis
* :code:`run_notebook.py` - Script to execute notebook programmatically

Configuration
*****************
The API server is configured to:

* Accept CORS requests from frontend applications
* Serve data in JSON format
* Handle real-time data fetching from external sources
* Process and filter data based on current conditions


Development
***********
To add new endpoints or modify data processing:

#. Edit api.py for new routes
#. Update data processing logic in the respective functions
#. Add new threshold files to Flooding_Thresholds/ as needed
#. Test endpoints using tools like Postman or curl

Deployment
**********
For production deployment:

#. Set up environment variables for API keys if needed
#. Configure proper CORS settings for your domain
#. Set up process management (PM2, systemd, etc.)
#. Configure reverse proxy (nginx) if needed
#. Set up SSL certificates for HTTPS

License
********
This project is developed for flood monitoring and public safety in the Waikāne area.
