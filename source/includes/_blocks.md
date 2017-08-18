# Blocks

## Get Hash of the Latest Block

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

### HTTP Request

`GET http://neoapi.net/v1/neo/asset/getBalanceById?asset_id={hash}`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
N/A | false | This endpoint requires no parameters.

## Get Index of the Latest Block

## Get the Latest Block

## Get Block By Hash

## Get Block By Index

