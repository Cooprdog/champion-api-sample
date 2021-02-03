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