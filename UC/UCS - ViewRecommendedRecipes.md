# Use-Case Specification: Get recommended Recipe

# 1. Get recommended Recipe

## 1.1 Brief Description
Find Recipes matching yur favorite Ingredients, which change every day or on user interaction

## 1.2 Mockup
n/a

## 1.3 Screenshot (Creation)
tbt since there not implemented yet, see mockups until further infos are given here.

# 2. Flow of Events

## 2.1 Basic Flow (Creation)
Here is the activity diagram for getting a recommendation.

## 2.2 Alternative Flows
A recommendation can be forced by pressing "refresh"

# 3. Special Requirements
n/a

# 4. Preconditions
The main preconditions for this use case are:

 1. The user has started the app and has navigated to "Home" section.

# 5. Postconditions

### 5.1 Save changes / Sync with server
n/a

# 6. Function Points
| View Recommended Recipes | RET | DET | FTR | Resulting Complexity | Count | RET | DET                | FTR    |
|--------------------------|-----|-----|-----|----------------------|-------|-----|--------------------|--------|
| External Inuts           | 0   | 1   | 0   | low                  | 1     |     | Recipe Detail Card |        |
| External Outputs         | 0   | 1   | 0   | low                  | 1     |     | Recipes            |        |
| External Inquiries       | 0   | 1   | 1   | low                  | 1     |     | Refresh Button     | Recipe |
| Internal Logical Files   | 0   | 0   | 0   | low                  | 0     |     |                    |        |
| External Interface Files | 0   | 0   | 0   | low                  | 0     |     |                    |        |
| Function Points          | 9,3 |