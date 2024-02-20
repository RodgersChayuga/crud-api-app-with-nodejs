## Introduction

This file defines a set of API endpoints for managing products in an Express application.

## Dependencies

This code assumes the existence of a Product model with appropriate methods for interacting with your product database.
Endpoints
GET /products
Retrieves all products from the database.

## Success Response:

#### Status code: 200

Content-Type: application/json
Body: JSON array of product objects
Error Response:

#### Status code: 500

Content-Type: application/json
Body: JSON object containing an error message
GET /products/:id
Retrieves a specific product by its ID.

## Success Response:

#### Status code: 200

Content-Type: application/json
Body: JSON object representing the product
Error Response:

#### Status code: 404

Content-Type: application/json
Body: JSON object containing an error message ("Product not found")

#### Status code: 500

Content-Type: application/json
Body: JSON object containing an error message
POST /products
Creates a new product based on the provided data in the request body.

## Success Response:

#### Status code: 200

Content-Type: application/json
Body: JSON object representing the created product
Error Response:

#### Status code: 500

Content-Type: application/json
Body: JSON object containing an error message
PUT /products/:id
Updates an existing product with the provided data in the request body.

## Success Response:

#### Status code: 200

Content-Type: application/json
Body: JSON object representing the updated product
Error Response:

#### Status code: 404

Content-Type: application/json
Body: JSON object containing an error message ("Product not found")

#### Status code: 500

Content-Type: application/json
Body: JSON object containing an error message
DELETE /products/:id
Deletes a specific product by its ID.

## Success Response:

#### Status code: 200

Content-Type: application/json
Body: JSON object containing a success message ("Product deleted successfully")
Error Response:

#### Status code: 404

Content-Type: application/json
Body: JSON object containing an error message ("Product not found")

#### Status code: 500

Content-Type: application/json
Body: JSON object containing an error message

## Notes

All error responses include a human-readable error message in the JSON body.
This is a basic example and can be extended to include additional features and functionalities specific to your application.
