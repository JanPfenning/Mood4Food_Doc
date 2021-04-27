# Use-Case Specification: Manage Settings

# 1. Manage Settings 

## 1.1 Brief Description
This use case allows the user to manage Settings concerning his health.
Bodyvariables like height or mass and further variables describing goals the user wants to reach.

## 1.2 Mockup
n/a

## 1.3 Screenshot (Creation)
tbt since there not implemented yet, see mockups until further infos are given here.

# 2. Flow of Events

## 2.1 Basic Flow (Creation)
Here is the activity diagram for managing bodymessure settings.

## 2.2 Alternative Flows
n/a

# 3. Special Requirements
n/a

# 4. Preconditions
The main preconditions for this use case are:

 1. The user has started the app and has navigated to "Recipe" section.

# 5. Postconditions

### 5.1 Save changes / Sync with server
bodymessures are stored in the local files (no information for the outside world!)

# 6. Function Points
| Manage Settings          | RET | DET | FTR | Resulting Complexity | Count | RET | DET                                                                                    | FTR      |
|--------------------------|-----|-----|-----|----------------------|-------|-----|----------------------------------------------------------------------------------------|----------|
| External Inuts           | 0   | 5   | 1   | low                  |       |     | Cur Body weight, Aim weight, Wheight Change, Wheight Change / Month, Physical Activity | Settings |
| External Outputs         | 0   | 0   | 0   | low                  |       |     |                                                                                        |          |
| External Inquiries       | 0   | 0   | 0   | low                  |       |     |                                                                                        |          |
| Internal Logical Files   | 0   | 0   | 1   | low                  |       |     |                                                                                        | Settings |
| External Interface Files | 0   | 0   | 0   | low                  |       |     |                                                                                        |          |
| Function Points          | 9,3 |