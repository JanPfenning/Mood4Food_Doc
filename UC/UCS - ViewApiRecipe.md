# Use-Case Specification: View API Recipe

# 1. View API Recipe

## 1.1 Brief Description
This use case allows users to read Recipes from the API.

## 1.2 Mockup
n/a

## 1.3 Screenshot (Creation)
tbt since there not implemented yet, see mockups until further infos are given here.

# 2. Flow of Events

## 2.1 Basic Flow (Creation)
Here is the activity diagram for reading a recipe from the API.

## 2.2 Alternative Flows
A recipe from the API could also be seen when recommendet

# 3. Special Requirements
n/a

# 4. Preconditions
The main preconditions for this use case are:

 1. The user has started the app and has navigated to "Recipe" section.

# 5. Postconditions

### 5.1 Save changes / Sync with server
n/a

# 6. Function Points
| View Api Recipes         | RET  | DET | FTR | Resulting Complexity | Count | RET     | DET                      | FTR    |
|--------------------------|------|-----|-----|----------------------|-------|---------|--------------------------|--------|
| External Inuts           | 0    | 2   | 1   | low                  | 2     |         | Search icon, Recipe Card | Recipe |
| External Outputs         | 1    | 0   | 0   | low                  | 1     | Recipes |                          |        |
| External Inquiries       | 0    | 1   | 1   | low                  | 1     |         | Input Field              | Recipe |
| Internal Logical Files   | 0    | 0   | 1   | low                  | 1     |         |                          | Recipe |
| External Interface Files | 0    | 0   | 0   | low                  | 0     |         |                          |        |
| Function Points          | 18,6 |