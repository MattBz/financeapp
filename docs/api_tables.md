# SmartBudget API Spec

## Categories
```json
{
  "data": [
    {
      "id": 1,
      "owner": "userid",
      "name": "Groceries",
      "position": 2,
      "isHidden": false
    }
  ]
}
```

## CategoryGroups
```json
{
  "data": [
    {
      "id": 1,
      "owner": "userid",
      "name": "Fixed Costs",
      "position": 2,
      "categories": [1,5,8]
    }
  ]
}
```

## Transactions
```json
{
  "data": [
    {
      "id": 1,
      "owner": "userid",
      "category": "categoryid",
      "amount": -50050,
      "date": "2017-04-16T22:48:39.330Z",
      "note": "Edeka",
      "repeatingType": 4,
      "lastDate": "2017-04-16T22:48:39.330Z"
    }
  ]
}
```

## RepeatingTypes
```json
{
  "data": [
    {
      "id": 1,
      "description": "Every 3 Months",
      "days": 0,
      "weeks": 0,
      "months: 3
    }
  ]
}
```

## Budgets
```json
{
  "data": [
    {
      "id": 1,
      "owner": "userid",
      "budgeted": 130000,
      "spent": 127400,   
      "income": 250000, 
      "toBeBudgeted": 150000,  
      "date": "2017-04-16T22:48:39.330Z",
      "budgetCategories": [
        {
          "id": 1,
          "category": "categoryid",
          "budgeted": 13000,
          "spent": 12550,    
          "carryOver": 200000          
        }
      ]
    }
  ]
}
```

### Category Table
id 
owner
categoryGroup
name
position
isHidden

### CategoryGroup Table
id
owner
name
position

### Transaction Table:
id
owner
category
amount
date
note
reaptingTypeId
lastDate

### Budget Table
id
owner
date
category
budgeted

### RepeatingTypes Tables
id
description
days
weeks
months
