# API Specification

## Accessibility

The Server is hosted on Strato.
API URL: http://irowall-tactical.com/mood4food/api

## Data Objects

### Recipe
- recipeId: int
- title: string
- description: string
- imageUri: string
- ingredients: Ingredient[]
- materials: Material[]

### Ingredient
- (materialId: int)
- name: string
- (recipeId: int)

### Material
- (materialId: int)
- name: string
- (recipeId: int)

## Endpoints

### GET /recipes[?recipeId|?limit|?offset|?search]
Request:
- Path Parameters: -
- Query Parameters:
  - Required: -
  - Optional:
    - recipeId (int): Specifies the one recipe which is returned.
    - limit (int): Specifies the maximum number of datasets returned.
    - offset (int): Specifies the number of datasets skipped for return.
    - search (string): Specifies a string which must be contained in the titles of all returned recipes.
- Headers: -
- Body: -

Response:
- Headers:
  - Content-Type: json/application; charset=utf-8
- Body:
  - Recipe[]
  - Recipe (if the recipeId parameter is present)

### GET /ingredients[?limit|?offset]
Request:
- Path Parameters: -
- Query Parameters:
  - Required: -
  - Optional:
    - limit (int): Specifies the maximum number of datasets returned.
    - offset (int): Specifies the number of datasets skipped for return.
- Headers: -
- Body: -

Response:
- Headers:
  - Content-Type: json/application; charset=utf-8
- Body:
  - Ingredient[]

### GET /materials[?limit|?offset]
Request:
- Path Parameters: -
- Query Parameters:
  - Required: -
  - Optional:
    - limit (int): Specifies the maximum number of datasets returned.
    - offset (int): Specifies the number of datasets skipped for return.
- Headers: -
- Body: -

Response:
- Headers:
  - Content-Type: json/application; charset=utf-8
- Body:
  - Material[]
