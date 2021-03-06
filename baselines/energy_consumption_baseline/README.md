# Energy Baselines

This app creates baselines of energy data (Green Button Meter) and presents the model accuracy (current implementation includes Linear Regression) and energy savings (both absolute & percentage)

Before running the app, edit the parameters in config.json,

- sites: Name of site. "" defaults to all sites in Green Button Meter. 
- time: start and end determine the range of data to query. Note: Use the format given in config.json to edit time.
- aggregation: Available aggregations include - pymortar.MEAN, pymortar.MAX, pymortar.MIN, pymortar.COUNT, pymortar.SUM, pymortar.RAW (the temporal window parameter is ignored)
- window: specifies the interval of data.
- time_features: specifies whether to use time_of_day and day_of_week to use for modeling energy consumption.
- separator: specifies the datetime post which energy savings need to be calculated.
- save_data: boolean variable to indicate whether to save data after querying mortar.

To run this app, execute the command,
python app.py

The app will print out the results in the terminal.
