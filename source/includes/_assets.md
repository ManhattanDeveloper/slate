# Assets

## Get Account Balance By ID

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

This endpoint returns the account balance of a given account.

### HTTP Request

`GET http://neoapi.net/v1/neo/asset/getBalanceById?asset_id={hash}`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
asset_id | true | The account ID (hash) of the account in question.
