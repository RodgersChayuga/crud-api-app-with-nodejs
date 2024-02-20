# This file defines a set of API endpoints for managing products in an Express application.

This result was from this tutorial: [CRUD App Backend](https://www.youtube.com/watch?v=_7UQPve99r4&t=1063s)

## Dependencies:

This code assumes the existence of a Product model with appropriate methods for interacting with your product database.
Endpoints:

## GET /products

Retrieves all products from the database.
Success response: Status code 200, JSON array of products.
Error response: Status code 500, JSON object with error message.

## GET /products/:id

Retrieves a specific product by its ID.
Success response: Status code 200, JSON object of the product.
Error response:
Status code 404: Product not found.
Status code 500: Internal server error.

## POST /products

Creates a new product based on the provided data in the request body.
Success response: Status code 200, JSON object of the created product.
Error response: Status code 500, JSON object with error message.

## PUT /products/:id

Updates an existing product with the provided data in the request body.
Success response: Status code 200, JSON object of the updated product.
Error response:
Status code 404: Product not found.
Status code 500: Internal server error.

## DELETE /products/:id

Deletes a specific product by its ID.
Success response: Status code 200, JSON object with success message.
Error response:
Status code 404: Product not found.
Status code 500: Internal server error.

## Notes:

All error responses include a human-readable error message in the JSON body.
This is a basic example and can be extended to include additional features and functionalities specific to your application.
