# Assignment_Comprinno


## Getting Started

1. Install Rails at the command prompt if you haven't yet:

        $ gem install rails


2. Change directory to `Assignment_Comprinno` and start the web server:

        $ cd Assignment_Comprinno
        $ rails server

4. Go to `http://localhost:3000` and you'll see:
"See API Documentation"


## API Documentation

These docs describe how to use the this API which are using rest call to display listing and crud features. 


### Create Product
```
URL:
	https://stormy-anchorage-59492.herokuapp.com/api/products

Request:
	Method: POST

Body:
	name : macbook
	price : 50000
	short_description : macbook 2018
```
	
#### Response:
```
Success:
{
   "status":"success"
}

Failure:
{"error":"price is missing, short_description is missing"}
```


### Read Product
```
URL:
	Get all product data https://stormy-anchorage-59492.herokuapp.com/api/products
	Get a single product data https://stormy-anchorage-59492.herokuapp.com/api/products/{id}


Request:
	Method: GET
	
```
#### Response:
```
Success:
{
    "id": 3,
    "name": "test",
    "price": "200.0",
    "short_description": "yash",
    "full_description": null,
    "created_at": "2019-04-23T18:35:49.636Z",
    "updated_at": "2019-04-23T18:35:49.636Z"
}

Failure:
{
    "status": "not_found"
}
```






### Update Product
```
URL:
	https://stormy-anchorage-59492.herokuapp.com/api/products/{id}

Request:
	Method: PUT

Body:
	name : macbook
	price : 52000
	short_description : macbook 2018
```

#### Response:
```
Success:
{"status":"success"}


Failure:
{"error":"name is missing, short_description is missing"}
```










### Delete Product
```
URL:
	https://stormy-anchorage-59492.herokuapp.com/api/products/{id}

Request:
	Method: DELETE
```


Response:
```
Success:
{
    "status": "success"
}


Failure:
{
    "error": "405 Not Allowed"
}
```
