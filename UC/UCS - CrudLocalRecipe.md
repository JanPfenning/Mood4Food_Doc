# Use-Case Specification: CRUD Recipe

# 1. CRUD Recipe

## 1.1 Brief Description
This use case allows users to create/read/update/delete own Recipes.
A Recipe holds information about ingrediends, materials and workflow.

## 1.2 Mockup
### Create recipe
https://konrad400294.invisionapp.com/public/prototype/skghts6bg00as9401o6extwkc
### Read recipe
n/a
### Update recipe
n/a
### Delete recipe
n/a


## 1.3 Screenshot

### 1.3.1 Creation
<img src="..\App-Screenshots\NewRecipe.PNG">

### 1.3.2 Read
<img src="..\App-Screenshots\View-API.PNG">

### 1.3.3 Update
<img src="..\App-Screenshots\Editing.PNG">

### 1.3.4 Delete
<img src="..\App-Screenshots\Deletion.PNG">

# 2. Flow of Events

## 2.1 Basic Flow
Users Usually create a recipe and review it later. they may update it or delete it from the phone.

## 2.1.1 Creation
Here is the activity diagram for adding a new recipe.

<a href="https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=createrecipe.drawio#Uhttps%3A%2F%2Fraw.githubusercontent.com%2FJanPfenning%2FMood4Food_Doc%2Fmain%2Fembedded-files%2Fcreaterecipe.drawio">Creating a Recipe Flow</a></p>

## 2.1.2 Read
User clicks on a Recipe-Card to see its Details

## 2.1.3 Update
See 2.1.1

## 2.1.4 Delete
On detail view a User may delete the recipe. He will be asked whether he is sure to do it or not.

## 2.2.1 Alternative Flows: Create
User is free in number of ingredients, materials and steps, as he is in whether a picture for the meal is added or not.

# 3. Special Requirements
n/a

# 4. Preconditions
The main preconditions for this use case are:

 1. The user has started the app and has navigated to "Recipe" section.

# 5. Postconditions

### 5.1 Create
New Recipe exists
The recipe is stored in the users local data
The User is at the detail information screen of the new recipe

### 5.2 View
n/a

### 5.3 Update
The recipe is stored in the users local data
The User is at the detail information screen of the edited recipe

### 5.1.3 Delete
The recipe is deleted and the user is navigated to Selection-Activity

# 6. Function Points
| CRUD Recipe                    | RET  | DET | FTR | Resulting Complexity | Count | RET                           | DET                                                                                                     | FTR    |
|--------------------------------|------|-----|-----|----------------------|-------|-------------------------------|---------------------------------------------------------------------------------------------------------|--------|
| External Inuts (EI)            | 3    | 9   | 1   | low                  | 3     | Ingredients, Materials, Steps | Name, Image, Ingredient Amount, Ingredient Name, Material, Step, Save, Cancel, Add Image, Delete Button | Recipe |
| External Outputs (EO)          | 0    | 1   | 0   | low                  | 1     |                               | Confirmation message                                                                                    | -      |
| External Inquiries (EQ)        | 0    | 0   | 0   | low                  | 0     |                               |                                                                                                         |        |
| Internal Logical Files (ILF)   | 0    | 0   | 0   | low                  | 1     |                               |                                                                                                         | Recipe |
| External Interface Files (EIF) | 0    | 0   | 0   | low                  | 0     |                               |                                                                                                         |        |
| Function Points                | 18,6 |