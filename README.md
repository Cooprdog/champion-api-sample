https://github.com/Cooprdog/champion-api-sample#status-codes-and-errors

# Resource Description: Find_champion
### Get all the champion data

# Sub Resources:
### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; name   &nbsp;&nbsp;&nbsp;role  &nbsp;&nbsp;&nbsp;  orign

# Description
### Querying this endpoint will return all the champions in the database as well as their role and their origin

# URL
### {Get} http(s)://Riotgames.com/find_champion

## Query Parameters


| Element       | Description | Type                   |
| ------------  | ----------  | -----------------------|        
| Champion_Data | Top Level          | Champion_Data_Object |
|   name        | champion name      | string               |
|   role        | champion position  | string               |
|   origin      | origin             | string               |

## Headers

| Header Name                    | Description        |
|--------------------------------|--------------------|
| Accept: application/json       |sets data format    |
| Content-type: application/json |sets data format    | 

## POST or PUT Body 
This is not applicable



## sample request

{GET} http(s)://Riotgames.com/find_champion

Accept: application/json

Content-type: application/json 

## Response

| Name           | Role          | Origin         |
|----------------|---------------|----------------|
| Ahri           | midlane       | vastaya        |
| Teemo          | top lane      | bandle city    |
| Gangplank      | top lane      | bilgewater     |
| Sona           | support       | ionia          |
| Miss Fortune   | marksman      | bilgewater     |

## Sample Response

```JSON
champion_data = [
{
   'name': 'ahri',
   'role':  'mid lane',
   'origin': 'vastaya'
 },
 {
   'name': 'teemo',
   'role': 'top lane',
   'origin': 'bandle city'
 },
 {
   'name':'gangplank',
   'role': 'top lane',
   'origin': 'bilgewater'
 },
 {
   'name': 'sona',
   'role': 'support',
   'origin': 'ionia'
 },
 {
   'name': 'miss fortune',
   'role': 'marksman',
   'origin': 'bilgewater'
 }
]
```

## Status Codes and Errors

### The following table lists HTTP status codes

| HTTP Status Code     |  Description             | 
|----------------------|--------------------------|
| 200                  | ok                       | 
| 400                  | Bad request              | 
| 401                  | unauthorized             | 
| 403                  |  Forbidden               | 
| 404                  | Data not found           | 
| 405                  | Method not allowed       | 
| 415                  | Unsupported media type   | 
| 429                  | Rate limit exceeded      |
| 500                  | Internal server error    |
| 502                  | Bad gateway              |
| 503                  | Service unavailable      |
| 504                  | Gateway timeout          |
