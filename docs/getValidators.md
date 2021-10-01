###### Endpoint

    https://boascan.io/validators?page=1&limit=1

HTTP Method: **GET**

Returns a set of Validators based on the block height if there is a height. If height was not provided the latest validator set is returned.

| Query String | Explanation    | Example                            |
| ------------ | ---------------- | -------------------------------------------- |
| page  | Page Number | 1 |
| ------------ | ---------------- | -------------------------------------------- |
| limit  | limit of Records | 1 |

Example Response JSON:<br/>
[{"address":"boa1xrval7gwhjz4k9raqukcnv2n4rl4fxt74m2y9eay6l5mqdf4gntnzhhscrh","enrolled_at":"0","stake":"0x210f6551d648a4da654da116b100e941e434e4f232b8579439c2ef64b04819bd2782eb3524c7a29c38c347cdf26006bccac54a58a58f103ae7eb5b252eb53b64","preimage":{"height":"","hash":"0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000"}}]