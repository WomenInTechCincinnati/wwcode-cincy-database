# wwcode-cincy-database

A starter project for Women Who Code Cincinnati Hacktoberfest project that serves
as a database

The available API endpoints and returned data can be viewed at  
http://my-json-server.typicode.com/WomenWhoCodeCincy/wwcode-cincy-database 

The structure of the returned json is described below 

[JsonLint](https://jsonlint.com/) is a useful (and free!) tool for validating your JSON structure

Full response:  
http://my-json-server.typicode.com/WomenWhoCodeCincy/wwcode-cincy-database/db

```
{
  "members": List<Member>,
  "quotes": List<Quote>,
  "learning_resources": List<LearningResource>,
  "women_who_code_cincinnati_information": ContactInformation
}
```
List of members:  
http://my-json-server.typicode.com/WomenWhoCodeCincy/wwcode-cincy-database/members

```
Member {
  "name": String,
  "image_url": String,
  "favorite_techs": List<String>,
  "hobbies": List<String>,
  "links": Links
}
```
where Links is defined as 
```
Links {
  "twitter": String,
  "facebook": String,
  "linkedIn": String,
  "website": String, 
  "github": String, 
  "meetup": String
}
```
List of Quotes:  
http://my-json-server.typicode.com/WomenWhoCodeCincy/wwcode-cincy-database/quotes

```
Quote {
  "submitted_by": String,
  "quote": String,
  "author": String
}
```
List of Learning Resources:  
http://my-json-server.typicode.com/WomenWhoCodeCincy/wwcode-cincy-database/learning_resources

```
LearningResource: {
  "submitted_by": String,
  "title": String,
  "short_description": String,
  "link": String,
  "topics": List<String>
}
```
Women Who Code Cincinnati Contact Information:  
http://my-json-server.typicode.com/WomenWhoCodeCincy/wwcode-cincy-database/women_who_code_cincinnati_information

```
ContactInformation {
  "links": Links,
  "email": String 
}
```
