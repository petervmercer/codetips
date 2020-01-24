# API Gateway

## Getting Started

### Creating a quick mock

####Steps
1. create a new API
2. Create a resourse
3. Create a Get method
4. make it a mock
5. Change the Integration response
6. Select the down arrow next 200 reponse
7. Choose Mapping templates
8. Then application/Json
9. add below json (fig 1.)
10. Choose to enable cors
11. Then deploy api

Fig 1.
```json
{
    "statusCode": "200",
    "body": "{'PK': 'USER','PR':'uuid-1'}"
    
}
```

