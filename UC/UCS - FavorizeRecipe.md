# Use-Case Specification: Favorize Recipe

# 1. Favorize Recipe

## 1.1 Brief Description
This Usecase allows the user to mark (API and local) recipes as favorites and find them more quickly.

## 1.2 Mockup
n/a

## 1.3 Screenshot
<img src="..\App-Screenshots\Favorization.PNG">

# 2. Flow of Events

## 2.1 Basic Flow
Here is the activity diagram for Toggle Favorite-State and for viewing the favorized Recipes.

<a href="https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=createrecipe.drawio#Uhttps%3A%2F%2Fraw.githubusercontent.com%2FJanPfenning%2FMood4Food_Doc%2Fmain%2Fembedded-files%2FfavorizeRecipe.drawio">Toggle Favorite State and view favorites</a></p>

## 2.2 Alternative Flows
The user can favorize a Recipe however he entered the Detailpage

# 3. Special Requirements
n/a

# 4. Preconditions
A Recipe must be existing

# 5. Postconditions

### 5.1 Save changes / Sync with server
The recipe id is saved to the local favorite recipe file

# 6. Function Points
| Favorize Recipes         | RET   | DET | FTR | Resulting Complexity | Count | RET | DET                 | FTR    |
|--------------------------|-------|-----|-----|----------------------|-------|-----|---------------------|--------|
| External Inuts           | 0     | 1   | 1   | low                  | 1     |     | Favorite Icon press | Recipe |
| External Outputs         | 0     | 1   | 0   | low                  | 1     |     | Favorite Icon       |        |
| External Inquiries       | 0     | 0   | 0   | low                  | 0     |     |                     |        |
| Internal Logical Files   | 0     | 0   | 1   | low                  | 1     |     |                     | Recipe |
| External Interface Files | 0     | 0   | 0   | low                  | 0     |     |                     |        |
| Function Points          | 13,02 |
