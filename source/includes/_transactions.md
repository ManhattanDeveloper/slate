# Transactions

## Get Transaction By Hash

```shell
curl "http://neoapi.net/v1/neo/asset/getBalanceById?asset_id=AS2H3RUV9fyHbzAFCfsrxkNMZ511rW7537"
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint returns the asset ID (hash) of the latest block on the chain.

## Get Transactions By Account (coming soon)