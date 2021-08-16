# Ability Test for Backend Developer Candidates

## Aims
As we have got to know you a little bit better in the last interview(s), we would like to give you the **opportunity** to:
- show us your skills, 
- give you a little bit of a taste of what is waiting for you.

Further this will **help** us to: 
- assess if we match
- determine how to include your skills as best as possible.

## Tasks
### 1. Create a "Development" environment
- You need a database
- Update this README.md and explain how to setup the environment

### 2. Create a microservice that achieves the following goals:
- the service **must**: 
  - store exchange data (date, currency, exchange rate) in a database
  - provide exchange data by
     - *date*: return a list of data where the date matches the given *date*
     - *currency*: return a list of data where the currency matches the given *currency*
     - *date* ***AND*** *currency*: return a list with one element where the date matches the given *date* and currency matches the given *currency*
  - provide an endpoint to receive a "FETCH" command. If the endpoint is called, the service begins to fetch and process data.
  - have been tested with mocked data. It is not mandatory to download data from [1] and [2] before or while tests are executed.

- The service **can**: 
   - process data as compressed CSV [1] or as XML [2]
   - use a “shareable” development environment	, by creating a docker-compose file where your required services are defined (e.g. database)
   - be dockerized
   - use Spring with Java or Kotlin (is a plus) to create the microservice
   - use MySQL [3] as database

### 3. Secure the Service
We use OAuth 2.0 with JWT (RS256).
- ensure all created endpoints are secured
- ensure there is a healthcheck endpoint that is not secured
- ensure all your tests still working
- use [4] as JWK URL
- you can use [5] as an external authorization service, where a new *Bearer* Token can requested using the credentials in [6]


### 4. Share your results
- Create a Pull Request.

## Links / References
[1] https://www.ecb.europa.eu/stats/eurofxref/eurofxref.zip (CSV (compressed))

[2] https://www.ecb.europa.eu/stats/eurofxref/eurofxref-daily.xml (XML)

[3] https://www.mysql.com

[4] https://auth.sandbox.api-ecolytiq.com/keys

[5] https://auth.sandbox.api-ecolytiq.com/oauth/token

[6] see credentials.txt

## Contacts
* [Daniel](mailto:daniel.quanz@ecolytiq.com)
* [Eric](mailto:eric.tessenow@ecolytiq.com)
* [Mirko](mailto:mirko.kaempf@ecolytiq.com)
