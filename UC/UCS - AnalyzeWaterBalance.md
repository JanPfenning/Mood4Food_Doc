# Use-Case Specification: Analyze Waterbalance

# 1. Analyze Waterbalance

## 1.1 Brief Description
This use case allows users to analyze past waterdata.

## 1.2 Mockup
n/a

## 1.3 Screenshot
### 
tbt since there not implemented yet, see mockups until further infos are given here.

# 2. Flow of Events

## 2.1 Basic Flow
Here is the activity diagram for retrieving the water history graph.

## 2.2 Alternative Flows
n/a

# 3. Special Requirements
To see meaningfull data you neet to have waterbalance data from the past

# 4. Preconditions
The main preconditions for this use case are:

 1. The user has started the app and has navigated to the "Water" section.

# 5. Postconditions

### 5.1 Save changes / Sync with server
The past waterdata is presented as a graph

# 6. Function Points
| Analyze Water            | RET   | DET | FTR | Resulting Complexity | Count | RET | DET                 | FTR   |
|--------------------------|-------|-----|-----|----------------------|-------|-----|---------------------|-------|
| External Inuts           | 0     | 1   | 0   | low                  | 1     |     | Navigation          |       |
| External Outputs         | 0     | 1   | 1   | low                  | 1     |     | Water history graph | Water |
| External Inquiries       | 0     | 0   | 0   | low                  | 0     |     |                     |       |
| Internal Logical Files   | 0     | 0   | 1   | low                  | 1     |     |                     | Water |
| External Interface Files | 0     | 0   | 0   | low                  | 0     |     |                     |       |
| Function Points          | 13,02 |