# Exercise

Implement an API for storing RSS feeds into a database.

## Specification
Your application should expose a following HTTP endpoint:

### API Definition: 

```
/analyse/new
```

### API Input:

This API endpoint should take at least two RSS URLs as a parameter (more are possible) e.g.:

https://news.google.com/news?cf=all&hl=en&pz=1&ned=us&output=rss

### API Response:

For each request executed against the API endpoint you should return an appropriate status (failed/success, etc)

### Workflow:

When the API is being called, your code should do a HTTP request to fetch the RSS feeds and process them in the following way:

Each item of the RSS feed should be stored in a database.

If the same item already exists, it should not be added into the database.

## Additional Information
You should use following frameworks for your work.

Spring JPA
H2 database running in memory (data will not be persistent across application restarts)
You are free to add / change any libraries which you might need to solve this exercise, the only requirement is that we do not have to setup / install any external software to run this application.

Running the exercise with maven

```mvn spring-boot:run```
