# Hawaii Vacation

## Climate Data
Used Python/Pandas to clean Hawaiian climate data and SQLalchemy to store. Mathplotlib allowed me to produce visualizations.

### API routes

* `/api/v1.0/precipitation`

  * Query for the dates and temperature observations from the last year.

* `/api/v1.0/stations`

  * Returns a json list of stations from the dataset.

* `/api/v1.0/tobs`

  * Returns a json list of Temperature Observations (tobs) for the previous year

* `/api/v1.0/<start>` and `/api/v1.0/<start>/<end>`

  * Return a json list of the minimum temperature, the average temperature, and the max temperature for a given start or start-end range.

  * When given the start only, calculates `TMIN`, `TAVG`, and `TMAX` for all dates greater than and equal to the start date.

  * When given the start and the end date, calculates the `TMIN`, `TAVG`, and `TMAX` for dates between the start and end date inclusive.

