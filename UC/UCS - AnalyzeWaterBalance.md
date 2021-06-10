# Use-Case Specification: Analyze Waterbalance

# 1. Analyze Waterbalance

## 1.1 Brief Description
This use case allows users to analyze past waterdata.

## 1.2 Mockup
n/a

## 1.3 Screenshot

<img src="..\App-Screenshots\AnalyzePastWater.PNG">


# 2. Flow of Events

## 2.1 Basic Flow
<a href="https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=Analyse_Waterbalance.drawio#R5Vpbc%2BI2FP41eQyjiyH2YzZJt5lpO5mhO9l9VLAAzxqLyiJAf30lLNmWZIMJty3hgbGOLpbO%2FXzyDX6Yrb5yMp%2F%2ByWKa3iAQr27w4w1CCEL5rwjrgtAPwoIw4UlckGBFGCb%2FUk0EmrpIYppbAwVjqUjmNnHEsoyOhEUjnLOlPWzMUvutczKhHmE4IqlPfU1iMS2oIbqr6L%2FTZDI1b4aDqOiZETNYnySfkpgtayT8dIMfOGOieJqtHmiqeGf4Usz7raW33Binmegy4e%2Fvz%2F%2B8rW8X9y%2Bz6PllMVz1v%2BDbvl7mnaQLfWK9W7E2LJDLSG7LxpepmKWSBuWjPM1c9eeCcDEURKj%2BcZKmDyxlfDMRg81PDRac%2FaS1nvFY9%2FiHMBuiXNBVjaQP9ZWyGRV8LYfo3ijqF1O0hmHN72UlLkOa1iRlaEQryKRcuOKhfNBs3IelqANLY6lkusm4mLIJy0j6VFHrrFasSKRG3qfJJJO0NyYEm8kOmsX3SsXVInOaFRRtQuFWtktu8%2FV3SQS9vmn%2BUE3TeFxZrbVutYpLasGEim1cwcVAdfKtUuU0JSJ5t82vSUh66gtL5F5KbYDAeA6tDrfIXqLYqZ5VNxdvIRD1otovtJbth%2FayOVvwEfWW3WhQeboDlAp7SnUvNWYtzRKBV2l9%2FI2kJBtRT9U4W2QxjbUuLaeJoMM5GanepfTYtqoRPtL6Eyhxj1kmmuzZsfOx%2FI1Ob%2Bd9W7B3oWfnEDUYenAyQ488mTwm%2BTwl608jEwgDWyhw4Hvf80pl0OR%2BB6l87Zc3Lp8mojz6Rx0y0Y44pWNxYv8MLe9cOesW%2F0xXidBuXeYhRVvNhD0AAt2upqpGfeYL5YkUAuW7vH3h7LYIAYKoa1yIOsYFrXG3oAejCNueQIv80NCBsZNJuDlCS%2ByQQt7YvBk2VwPybS8KHauB4fZY5E0IrVxPPhR7aJ7u2OgtdEIiG49zepKwNQg8Y%2FyDkVjVA0SQTT7OlT7RVObuVNGXlP68Yn%2BJnSBW1jkX85cme%2F6V09VWzp88m0TQdglVwNs7n9y91IlzSJkadxB1JaSMZUq0Mcmnpe3V5PxxodR0vd%2Bg6oZ2qOxkBm8xPILd%2BL17JXehFh04nuC6lJTXIzjslHAR%2Bqjg8NYa7uxi9Iu4b7nMtlxRymAiHLTFco1avvUIpkkmMx1J0ao0znPGsySONw67KYhWYfZo0Eyz3dT0KGjQI1fcR4t1EPj5yLfn6%2BU%2FhA42dnkB%2BNnGcJ0LOrtiIeBfzgoGHcLJpRFKXcnCWhWr69%2F2GrZENfermluFvLPONbDczjK3LIhPnrFCp8KIHKCyO%2F6JHLVF54U8IQiPrKZnwG0M%2FvIRrd0T6zlAa7uCM9C4qj3QmTCEkaU3%2BEjoDBg4%2Bhh2S9%2Fa0ZlW3Ud21DQ3Ou14SZP1OFhSx%2BLjeNbjo9NN0MtowTcKhMDrlSMv2Fafi18flMZVk9Bf5D2ZqLtUaZxT5YEKQCy%2FXrm4tzqXv0CABh79P6RHVXD5UUuWmgPNxwNG9zhwcOnv4qMdIfgGB%2BxC5qBb%2BrI3mO9eOJstt4MSLWdsBPOPFg%2BgDz58ynuxM5iLufXokF8Fe%2BdXJ7v9Qne2WuIA9sIAVD98YLrV8t4Auu9F2%2B0HDbZOOPplWMOWQdhDNpaI3Gz01Pkd9KGsT%2F%2F1AUYXTx6An9T5TnXbB3XKFV7yczoIncDZBz5Tz%2FpBnbkdv5LQtecnd%2BfO9DrHLtA1J7xE7Op3Sxv3DlbIuQnE4Y5kz0Xg8Ym%2F3GgIVg6OV4bPgyOVbFafLxfDq2%2FA8dN%2F
"> here </a> is the activity diagram for retrieving the water history graph.

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