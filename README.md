


1) Extract Source Data
  *We pulled csv our source data files freom Kaggle as follows:

  *Hospital beds: https://www.kaggle.com/ikiulian/global-hospital-beds-capacity-for-covid19
  *Covid 19 State and County files: https://www.kaggle.com/sudalairajkumar/covid19-in-usa



2)Transform Data (Cleanup and Analysis)
  We had to clean one of the csv data files in excel just a bit before loading it into the jupyter notebook as one file only had full state name and one had only the two digit postal code name for the state. We loaded the csv files into a jupyter notebook, creating a dataframe from each. We then began the cleanup as follows:

  *Hospital beds df:
  dropped unnecessary columns

  *Covid States df:
  dropped unnecessary columns
  merged with Covid Counties df
  renamed a few columns





3)Load Data into Postres Database
 *We created a database named covid_db with the following tables:

  locations
  avail_hospital_beds
  cases
  Used SQLAlchemy to load our data into the our Postgres Database
