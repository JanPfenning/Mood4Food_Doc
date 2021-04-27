# Use-Case Specification: Rate Ingredients

# 1. Rate Ingredients 

## 1.1 Brief Description
This use case allows users to like or dislike ingredients so they will not appear in recommended searches

## 1.2 Mockup
n/a

## 1.3 Screenshot (Creation)
tbt since there not implemented yet, see mockups until further infos are given here.

# 2. Flow of Events

## 2.1 Basic Flow (Creation)
Here is the activity diagram for rating an ingredient.

## 2.2 Alternative Flows
n/a

# 3. Special Requirements
n/a

# 4. Preconditions
The main preconditions for this use case are:

 1. The user has started the app and has navigated to "Settings" section.

# 5. Postconditions

### 5.1 Save changes / Sync with server
Ingredient rating is stored in the local files (no access from outside the phone)

# 6. Function Points
| Rate Ingredients         | RET   | DET | FTR | Resulting Complexity | Count | RET | DET          | FTR      |
|--------------------------|-------|-----|-----|----------------------|-------|-----|--------------|----------|
| External Inuts           | 0     | 1   | 1   | low                  | 2     |     | Like/Dislike | Settings |
| External Outputs         | 0     | 0   | 0   | low                  | 0     |     |              |          |
| External Inquiries       | 0     | 1   | 1   | low                  | 1     |     | Input        | Settings |
| Internal Logical Files   | 0     | 0   | 1   | low                  | 1     |     |              | Settings |
| External Interface Files | 0     | 0   | 0   | low                  |       |     |              |          |
| Function Points          | 14,88 |