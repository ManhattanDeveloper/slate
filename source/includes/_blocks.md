# Blocks

## Get Hash of the Latest Block

```shell
curl "http://neoapi.net/v1/block/getLatestBlockHash"
```

> The above command returns JSON structured like this:

```json
{
  "hash": "d211efb8d868ec764a1390247e89636edf7fc7b18132e0ed92c421173d7a7b70"
}
```

This endpoint returns the asset ID (hash) of the latest block on the chain.

### HTTP Request

`GET http://neoapi.net/v1/block/getLatestBlockHash`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
N/A | false | This endpoint requires no parameters.








## Get Index of the Latest Block

```shell
curl "http://neoapi.net/v1/block/getLatestBlockIndex"
```

> The above command returns JSON structured like this:

```json
{
  "index": 1267087
}
```

This endpoint returns the asset ID (hash) of the latest block on the chain.

### HTTP Request

`GET http://neoapi.net/v1/block/getLatestBlockIndex`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
N/A | false | This endpoint requires no parameters.







## Get the Latest Block

```shell
curl "http://neoapi.net/v1/block/getLatestBlock"
```

> The above command returns JSON structured like this:

```json
{
  "jsonrpc": "2.0",
  "id": 456,
  "result": {
    "hash": "0a26b41c77c4a572b069f2e6ca969af074bc5780f7856941b031287fbec98f5c",
    "size": 1531,
    "version": 0,
    "previousblockhash": "38f5a61ecae0d6fd6f2cc2c22db1f9fbf8d572d0daa2de52b6d04e95ec7cf0c0",
    "merkleroot": "90d445081a430d357b0be4ead5b56a9f7e1770308841f77b7c30ecf397ff7acf",
    "time": 1503117639,
    "index": 1267148,
    "nonce": "cedea8db110f2e42",
    "nextconsensus": "APyEx5f4Zm4oCHwFWiSTaph1fPBxZacYVR",
    "script": {
      "invocation": "40bcb9219b472c5823a1ae7be32b1cbe768c1e4a164b86429b4e97e9356efe133a2172af058c9f8ccbb8ef9ba5f6282ca84cf8d5d3ac1dc275a85382f0f1d8db2f40f7ddeaf24de58d786db2ea4ba0907d2f868958fae8c9b6c2e4f6ee75466f8a05e8d64fe0a0190302deca00b446946643930954d8431e1de029acca002b05f862400c98b4ef805d990c6401483482817ba6261cb25479391944034d40b451c25872231060cb60f48a888546a5a41f5b77a13a6b3d2cd839e23928b31c7fcaa7e6db40847425be396c63a210a67a986668293fb8d380cc1c3b6ba0ddefbd5fe3ed0457d1da796ce3525ebfda9b8606632890860a1b99cd59eaa11145d60a1d6c9890914083a8a87b71a349ded7b340052b16ea8c4a8b9391ddb55a2be5c33e7aacf4de28a50c3b06e98cfef3173cfbe0597d474e33bf60296f6145de3b9da45be8786cd7",
      "verification": "552102486fd15702c4490a26703112a5cc1d0923fd697a33406bd5a1c00e0013b09a7021024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d2102aaec38470f6aad0042c6e877cfd8087d2676b0f516fddd362801b9bd3936399e2103b209fd4f53a7170ea4444e0cb0a6bb6a53c2bd016926989cf85f9b0fba17a70c2103b8d9d5771d8f513aa0869b9cc8d50986403b78c6da36890638c3d46a5adce04a2102ca0e27697b9c248f6f16e085fd0061e26f44da85b58ee835c110caa5ec3ba5542102df48f60e8f3e01c48ff40b9b7f1310d7a8b2a193188befe1c2e3df740e89509357ae"
    },
    "tx": [
      {
        "txid": "fbf988b6a9b681891287f181243f10d4c9a4f8e0be38a3731dee4e7f6a0df731",
        "size": 10,
        "type": "MinerTransaction",
        "version": 0,
        "attributes": [],
        "vin": [],
        "vout": [],
        "sys_fee": "0",
        "net_fee": "0",
        "scripts": [],
        "nonce": 286207554
      },
      {
        "txid": "45645f5bf11c24d8c12cb6f9081f1634eb87533d64f36ff3ce5a6ca51b82d510",
        "size": 237,
        "type": "ClaimTransaction",
        "version": 0,
        "attributes": [],
        "vin": [],
        "vout": [
          {
            "n": 0,
            "asset": "602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7",
            "value": "0.00100608",
            "address": "AMqtjGEdkKiGP75LbdPGqt6uUPdGnP4nLf"
          }
        ],
        "sys_fee": "0",
        "net_fee": "0",
        "scripts": [
          {
            "invocation": "4066b4ebd3f4be05f43055a3e88352d531305726ce2ac7d4cfde1acb1d2dc0e174ea3e97285d7b666e7e8c5bbbe3880e95c16025418073853deda1952e7c78b373",
            "verification": "2103893dfd985112643e38b5e8e9980c9fa3783c4cb66341861a82e40239c53c47e2ac"
          }
        ],
        "claims": [
          {
            "txid": "9d04903633f7da67e6057530d1216772292ee6df94800d40859ba2df043be2b7",
            "vout": 0
          },
          {
            "txid": "b5923908437352aa73bc928218c9199d76234da117c4e71d678c80eff6e457cd",
            "vout": 0
          }
        ]
      }
    ],
    "confirmations": 1
  }
}
```

This endpoint returns the latest block on the chain.

### HTTP Request

`GET http://neoapi.net/v1/block/getLatestBlock`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
N/A | false | This endpoint requires no parameters.











## Get Block By Hash
```shell
curl "http://neoapi.net/v1/block/getBlockByHash?hash=0a26b41c77c4a572b069f2e6ca969af074bc5780f7856941b031287fbec98f5c"
```

> The above command returns JSON structured like this:

```json
{
  "jsonrpc": "2.0",
  "id": 456,
  "result": {
    "hash": "0a26b41c77c4a572b069f2e6ca969af074bc5780f7856941b031287fbec98f5c",
    "size": 1531,
    "version": 0,
    "previousblockhash": "38f5a61ecae0d6fd6f2cc2c22db1f9fbf8d572d0daa2de52b6d04e95ec7cf0c0",
    "merkleroot": "90d445081a430d357b0be4ead5b56a9f7e1770308841f77b7c30ecf397ff7acf",
    "time": 1503117639,
    "index": 1267148,
    "nonce": "cedea8db110f2e42",
    "nextconsensus": "APyEx5f4Zm4oCHwFWiSTaph1fPBxZacYVR",
    "script": {
      "invocation": "40bcb9219b472c5823a1ae7be32b1cbe768c1e4a164b86429b4e97e9356efe133a2172af058c9f8ccbb8ef9ba5f6282ca84cf8d5d3ac1dc275a85382f0f1d8db2f40f7ddeaf24de58d786db2ea4ba0907d2f868958fae8c9b6c2e4f6ee75466f8a05e8d64fe0a0190302deca00b446946643930954d8431e1de029acca002b05f862400c98b4ef805d990c6401483482817ba6261cb25479391944034d40b451c25872231060cb60f48a888546a5a41f5b77a13a6b3d2cd839e23928b31c7fcaa7e6db40847425be396c63a210a67a986668293fb8d380cc1c3b6ba0ddefbd5fe3ed0457d1da796ce3525ebfda9b8606632890860a1b99cd59eaa11145d60a1d6c9890914083a8a87b71a349ded7b340052b16ea8c4a8b9391ddb55a2be5c33e7aacf4de28a50c3b06e98cfef3173cfbe0597d474e33bf60296f6145de3b9da45be8786cd7",
      "verification": "552102486fd15702c4490a26703112a5cc1d0923fd697a33406bd5a1c00e0013b09a7021024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d2102aaec38470f6aad0042c6e877cfd8087d2676b0f516fddd362801b9bd3936399e2103b209fd4f53a7170ea4444e0cb0a6bb6a53c2bd016926989cf85f9b0fba17a70c2103b8d9d5771d8f513aa0869b9cc8d50986403b78c6da36890638c3d46a5adce04a2102ca0e27697b9c248f6f16e085fd0061e26f44da85b58ee835c110caa5ec3ba5542102df48f60e8f3e01c48ff40b9b7f1310d7a8b2a193188befe1c2e3df740e89509357ae"
    },
    "tx": [
      {
        "txid": "fbf988b6a9b681891287f181243f10d4c9a4f8e0be38a3731dee4e7f6a0df731",
        "size": 10,
        "type": "MinerTransaction",
        "version": 0,
        "attributes": [],
        "vin": [],
        "vout": [],
        "sys_fee": "0",
        "net_fee": "0",
        "scripts": [],
        "nonce": 286207554
      },
      {
        "txid": "45645f5bf11c24d8c12cb6f9081f1634eb87533d64f36ff3ce5a6ca51b82d510",
        "size": 237,
        "type": "ClaimTransaction",
        "version": 0,
        "attributes": [],
        "vin": [],
        "vout": [
          {
            "n": 0,
            "asset": "602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7",
            "value": "0.00100608",
            "address": "AMqtjGEdkKiGP75LbdPGqt6uUPdGnP4nLf"
          }
        ],
        "sys_fee": "0",
        "net_fee": "0",
        "scripts": [
          {
            "invocation": "4066b4ebd3f4be05f43055a3e88352d531305726ce2ac7d4cfde1acb1d2dc0e174ea3e97285d7b666e7e8c5bbbe3880e95c16025418073853deda1952e7c78b373",
            "verification": "2103893dfd985112643e38b5e8e9980c9fa3783c4cb66341861a82e40239c53c47e2ac"
          }
        ],
        "claims": [
          {
            "txid": "9d04903633f7da67e6057530d1216772292ee6df94800d40859ba2df043be2b7",
            "vout": 0
          },
          {
            "txid": "b5923908437352aa73bc928218c9199d76234da117c4e71d678c80eff6e457cd",
            "vout": 0
          }
        ]
      }
    ],
    "confirmations": 1
  }
}
```

This endpoint returns a block based on a given hash.

### HTTP Request

`GET http://neoapi.net/v1/block/getBlockByHash?hash={block_hash}`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
hash | true | The hash of the desired block.



## Get Block By Index

```shell
curl "http://neoapi.net/v1/block/getBlockByIndex?index=1267148"
```

> The above command returns JSON structured like this:

```json
{
  "jsonrpc": "2.0",
  "id": 456,
  "result": {
    "hash": "0a26b41c77c4a572b069f2e6ca969af074bc5780f7856941b031287fbec98f5c",
    "size": 1531,
    "version": 0,
    "previousblockhash": "38f5a61ecae0d6fd6f2cc2c22db1f9fbf8d572d0daa2de52b6d04e95ec7cf0c0",
    "merkleroot": "90d445081a430d357b0be4ead5b56a9f7e1770308841f77b7c30ecf397ff7acf",
    "time": 1503117639,
    "index": 1267148,
    "nonce": "cedea8db110f2e42",
    "nextconsensus": "APyEx5f4Zm4oCHwFWiSTaph1fPBxZacYVR",
    "script": {
      "invocation": "40bcb9219b472c5823a1ae7be32b1cbe768c1e4a164b86429b4e97e9356efe133a2172af058c9f8ccbb8ef9ba5f6282ca84cf8d5d3ac1dc275a85382f0f1d8db2f40f7ddeaf24de58d786db2ea4ba0907d2f868958fae8c9b6c2e4f6ee75466f8a05e8d64fe0a0190302deca00b446946643930954d8431e1de029acca002b05f862400c98b4ef805d990c6401483482817ba6261cb25479391944034d40b451c25872231060cb60f48a888546a5a41f5b77a13a6b3d2cd839e23928b31c7fcaa7e6db40847425be396c63a210a67a986668293fb8d380cc1c3b6ba0ddefbd5fe3ed0457d1da796ce3525ebfda9b8606632890860a1b99cd59eaa11145d60a1d6c9890914083a8a87b71a349ded7b340052b16ea8c4a8b9391ddb55a2be5c33e7aacf4de28a50c3b06e98cfef3173cfbe0597d474e33bf60296f6145de3b9da45be8786cd7",
      "verification": "552102486fd15702c4490a26703112a5cc1d0923fd697a33406bd5a1c00e0013b09a7021024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d2102aaec38470f6aad0042c6e877cfd8087d2676b0f516fddd362801b9bd3936399e2103b209fd4f53a7170ea4444e0cb0a6bb6a53c2bd016926989cf85f9b0fba17a70c2103b8d9d5771d8f513aa0869b9cc8d50986403b78c6da36890638c3d46a5adce04a2102ca0e27697b9c248f6f16e085fd0061e26f44da85b58ee835c110caa5ec3ba5542102df48f60e8f3e01c48ff40b9b7f1310d7a8b2a193188befe1c2e3df740e89509357ae"
    },
    "tx": [
      {
        "txid": "fbf988b6a9b681891287f181243f10d4c9a4f8e0be38a3731dee4e7f6a0df731",
        "size": 10,
        "type": "MinerTransaction",
        "version": 0,
        "attributes": [],
        "vin": [],
        "vout": [],
        "sys_fee": "0",
        "net_fee": "0",
        "scripts": [],
        "nonce": 286207554
      },
      {
        "txid": "45645f5bf11c24d8c12cb6f9081f1634eb87533d64f36ff3ce5a6ca51b82d510",
        "size": 237,
        "type": "ClaimTransaction",
        "version": 0,
        "attributes": [],
        "vin": [],
        "vout": [
          {
            "n": 0,
            "asset": "602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7",
            "value": "0.00100608",
            "address": "AMqtjGEdkKiGP75LbdPGqt6uUPdGnP4nLf"
          }
        ],
        "sys_fee": "0",
        "net_fee": "0",
        "scripts": [
          {
            "invocation": "4066b4ebd3f4be05f43055a3e88352d531305726ce2ac7d4cfde1acb1d2dc0e174ea3e97285d7b666e7e8c5bbbe3880e95c16025418073853deda1952e7c78b373",
            "verification": "2103893dfd985112643e38b5e8e9980c9fa3783c4cb66341861a82e40239c53c47e2ac"
          }
        ],
        "claims": [
          {
            "txid": "9d04903633f7da67e6057530d1216772292ee6df94800d40859ba2df043be2b7",
            "vout": 0
          },
          {
            "txid": "b5923908437352aa73bc928218c9199d76234da117c4e71d678c80eff6e457cd",
            "vout": 0
          }
        ]
      }
    ],
    "confirmations": 1
  }
}
```

This endpoint returns a block based on a given index.

### HTTP Request

`GET http://neoapi.net/v1/block/getBlockByIndex?index={block_index}`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
index | true | The index of the desired block.



## Get Indices by Time Range (coming soon)


