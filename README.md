# Time-series-stuck-pipe-prediction
This is a preliminary dataset obtained after the development of the Volve field dataset:https://www.equinor.com/en/news /14jun2018-disclosing-volve-data.html
The time-based benchmark is established first, the international standard time format of raw drilling temporal data is converted to a time format supported by pandas.
To ensure accuracy, the millisecond information is round to the nearest second-level, considering that most millisecond values were either greater than 900 milliseconds or less than 100 milliseconds. 
Due to the presence of unusable time interval data in the raw drilling data, which holds poor significance for stuck pipe prediction, we manually remove these segments from the time series.
