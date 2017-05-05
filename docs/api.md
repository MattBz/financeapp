# Financeapp API Spec

## Accounts
```json
{
  "accounts": [{
    "id": 1,
    "name": "DIBA",
    "balance": 12500.23,
    "owner": "username",
    "sharedUser": [
      "username2",
      "username3"
    ]
  }]
}
```

## Transaction
```json
{
  "transactions": [{
    "id": 1,
    "value": -500.50,
    "categorie": {
      "id": 2,
      "name": "Lebensmittel",        
    },
    "note": "Edeka"
  }]
}
```

## Categories
```json
{
  "categories": [{
    "id": 1,
    "name": "Essen",
    "subcategories": [
      {
        "id": 2,
        "name": "Lebensmittel",
        "subcategories" : []
      }, 
      {
        "id": 3,
        "name": "Restaurantbesuche",
        "subcategories" : []        
      }
    ]
  }]
}
```

## Income


## Bills


## Projects





`GET /:userid/accounts`

## Version 1
* Login (E-Mail / Password)
* Dashboard (Overview, Net worth, Basic Charts)
* Account
  * Shared Accounts
* Categories
  * Subcategories
* Bills
* Projects
* Import
  * Assign transactions
  * Fixed DIBA layout
