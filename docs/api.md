# Financeapp API Spec

## Transaction
```json
{
  "transactions": [
    {
      "id": 1,
      "value": -500.50,
      "categorie": 2,
      "note": "Edeka"
    }
  ]
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

## Budget
```json
{
  "budgets": [{
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

## Income


## Bills


## Projects





`GET /transactions`

## Version 1
* Login (E-Mail / Password)
* Dashboard (Overview, Net worth, Basic Charts)
* Categories
  * Subcategories
* Bills
* Projects
* Import
  * Assign transactions
  * Fixed DIBA layout
