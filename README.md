# FlaskApi

Used In-memory api or stored entire csv as a python global variable in json form.

GET Requests
-------------------- 

/historical -- to get all available dates


/historical/YYYYMMDD -- to get data related to given date (Input can be passed through url)


/forecast/YYYYMMDD -- to get weather data of next 5 days(Input can be passed through url)


POST Request
-----------------
historical/JSON as headers -- to post data related to a particular date(Input to be passed in json as header)
-- Checked for all history of this date and removed them(Handled duplicated insert condition)


DELETE Request
------------------
/historical/YYYYMMDD -- to delete all available data of this date.(Input to be passed in header)
Also checked and deleted duplicate data avaialable for given date


