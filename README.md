## ERP Integration Service (Micro Integrator)

### GET Request
```
curl 'http://localhost:8290/aggregate/data/90090087'
```

### GET Response
```
{
    "productDetails": {
        "id": "90090087",
        "name": "T Shirt",
        "description": "Test Shirt",
        "price": {
            "currency": "USD",
            "amount": 90.1
        }
    },
    "inventory": {
        "productId": "90090087",
        "quantity": 11
    }
}
```

### POST Request
```
curl --location 'http://localhost:8290/aggregate/data' \
--header 'Content-Type: application/json' \
--data '{
	"id": "90090087"
}'
```

### POST Response
```
{
    "message": "Successfully Inserted Product Inventory Data"
}
```
