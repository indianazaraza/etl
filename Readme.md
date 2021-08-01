# Readme

This project takes data from the [Jikan API](https://jikan.moe/), processes and cleans it using Pandas and transfers it to two databases: PostgreSQL and MariaDB with SQLAlchemy.
For more details about your api, read its documentation.
For more details about SQLAlchemy and drivers: [documentation](https://docs.sqlalchemy.org/en/14/dialects/index.html).
Problems you probably have with databases and SQLAlchemy:

1. When you install sqlalchemy, restart the session to the jupyter notebook; otherwise it won't work.

2. When you install psycopg2-binary on Linux, you may get errors about some packages that you have not installed. Watch these answers on [Stackoverflow](https://stackoverflow.com/questions/5420789/how-to-install-psycopg2-with-pip-on-python) or this video on [Youtube](https://www.youtube.com/watch?v=SM8YqCy2W8o) or copy the code in your terminal:
~~~
	sudo apt install gcc g++ build-essential
	sudo apt install python3.8-dev libpq-dev
	python3 -m pip install psycopg2
~~~
If that doesn't work restart the session to the jupyter notebook

3. When you transfer the data frame to the databases, you must have created the databases, not the tables.


