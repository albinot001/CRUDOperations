## API Endpoint Explanation

We have 4 CRUD operations: create, display, update, and delete.

For their functionality, everything is set in the controller. The functions were tested with Postman. Here’s how you can test them:

### Get All Data
If we look to get all the data back, it will return empty because we haven't added anything yet. You can test it out with this endpoint:
```
http://localhost:8000/api/products
```
(Note: `8000` is my local port; yours may differ.) You should get a `200` response back but with an empty result.

### Create a Product
To create a product, use the same endpoint but make a POST request in Postman. Add data in JSON format in the body (raw):
```json
{
  "name": "Product 2",
  "description": "Description",
  "price": 10.99
}
```

### Delete a Product
To delete a product, use this endpoint:
```
http://localhost:8000/api/products/1
```
(Here, `1` is the ID of the product.) If you're unsure of the ID, use the GET endpoint to retrieve the product data and check the ID.

### Update a Product
For updating a product (PUT request in Postman), use the same endpoint as delete:
```
http://localhost:8000/api/products/1
```
We assume you want to update a product that already exists. Add the same data as the POST method and change some values (not the variable names). If the request works, you can use the GET method to confirm the updated data.



