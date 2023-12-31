# sqlalchemy-challenge

Climate Analysis and Exploration

This project used a Python and SQLAlchemy to make climate analysis, and data exploration of the climate database. All of the following analysis completed by using SQLAlchemy ORM queries, Pandas, and Matplotlib. The complete climate analysis, and data exploration with python pandas notebook file found here starter notebook, and the SQLAlchemy file is also provided here hawaii.sqlite.

SQLAlchemy engin created create_engine to connect to the sqlite database. engine = create_engine("sqlite:///Resources/hawaii.sqlite") inspector = inspect(engine)`

To reflect the tables into classes, and save a reference to those classes called Station and Measurement an SQLAlchemy automap_base() is used.

Precipitation Analysis

A query is designed to retrieve the last 12 months of precipitation data, and only the date and prcp values is slected.

The query results also loded into a Pandas DataFrame and the index is seted in to the date column, and sorted the DataFrame values by date.

Finally the result ploted by using the DataFrame plot method.The plot looks as follows:

![image](https://github.com/MdataHolman/sqlalchemy-challenge/assets/147290574/38073009-1a3f-472e-87ab-b057f16244e2)

