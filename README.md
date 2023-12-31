# sqlalchemy-challenge

Climate Analysis and Exploration

This project used Python and SQLAlchemy to make climate analysis and data exploration of the climate database—all of the following analyses were completed by using SQLAlchemy ORM queries, Pandas, and Matplotlib. The complete climate analysis, data exploration with the Python pandas notebook file is found here starter notebook, and the SQLAlchemy file is also provided here hawaii.sqlite.

SQLAlchemy engine created create_engine to connect to the sqlite database. engine = create_engine("sqlite:///Resources/Hawaii.sqlite") inspector = inspect(engine)`

To reflect the tables into classes, and save a reference to those classes called Station and Measurement an SQLAlchemy automap_base() is used.

Precipitation Analysis

A query is designed to retrieve the last 12 months of precipitation data, and only the date and prcp values are selected.

The query results are also loaded into a Pandas DataFrame and the index is set into the date column, and the DataFrame values by date.

Finally, the result is plotted by using the DataFrame plot method. The plot looks as follows:

![image](https://github.com/MdataHolman/sqlalchemy-challenge/assets/147290574/38073009-1a3f-472e-87ab-b057f16244e2)

Station Analysis
A query is designed to calculate the total number of stations, and 9 stations found. To find the most active station list, and observation counts is sorted in descending order. Station USC00519281 has the highest number of observations.

A query is created to retrieve the last 12 months of temperature observation data (TOBS) and filter by the station with the highest number of observations. The Plot for the results as a histogram with bins=12 was created and it looks as follows.
