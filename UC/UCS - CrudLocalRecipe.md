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


## 1.3 Screenshot (Creation)
### 
tbt since there not implemented yet, see mockups until further infos are given here.

# 2. Flow of Events

## 2.1 Basic Flow (Creation)
Here is the activity diagram for adding a new recipe.

<iframe frameborder="0" style="width:100%;height:782px;" src="https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=createrecipe.drawio#Uhttps%3A%2F%2Fraw.githubusercontent.com%2FJanPfenning%2FMood4Food_Doc%2Fmain%2Fembedded-files%2Fcreaterecipe.drawio"></iframe>
</br>
<p style="font-size:0.8rem">
Use the following link to see the diagramm when the iframe doesn't work:</br>
<a href="https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=createrecipe.drawio#Uhttps%3A%2F%2Fraw.githubusercontent.com%2FJanPfenning%2FMood4Food_Doc%2Fmain%2Fembedded-files%2Fcreaterecipe.drawio">Creating a Recipe Flow</a></p>

## 2.2 Alternative Flows
User is free in number of ingredients, materials and steps, as he is in whether a picture for the meal is added or not.

# 3. Special Requirements
n/a

# 4. Preconditions
The main preconditions for this use case are:

 1. The user has started the app and has navigated to "Recipe" section.

# 5. Postconditions

### 5.1 Save changes / Sync with server
The recipe is stored in the users local data

# 6. Function Points
| CRUD Recipe                    | RET  | DET | FTR | Resulting Complexity | Count | RET                           | DET                                                                                                     | FTR    |
|--------------------------------|------|-----|-----|----------------------|-------|-------------------------------|---------------------------------------------------------------------------------------------------------|--------|
| External Inuts (EI)            | 3    | 9   | 1   | low                  | 3     | Ingredients, Materials, Steps | Name, Image, Ingredient Amount, Ingredient Name, Material, Step, Save, Cancel, Add Image, Delete Button | Recipe |
| External Outputs (EO)          | 0    | 1   | 0   | low                  | 1     |                               | Confirmation message                                                                                    | -      |
| External Inquiries (EQ)        | 0    | 0   | 0   | low                  | 0     |                               |                                                                                                         |        |
| Internal Logical Files (ILF)   | 0    | 0   | 0   | low                  | 1     |                               |                                                                                                         | Recipe |
| External Interface Files (EIF) | 0    | 0   | 0   | low                  | 0     |                               |                                                                                                         |        |
| Function Points                | 18,6 |