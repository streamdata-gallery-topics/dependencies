swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/listings/stock_dependence_types:
    get:
      summary: List listing stock dependence types
      description: Lists listing stock dependence types.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-types-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Stock
      - Dependence
      - Types
  /rest/listings/stock_dependence_types/{id}:
    get:
      summary: Get a listing stock dependence type
      description: Gets a listing stock dependence type by given ID.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-typesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Stock
      - Dependence
      - Type