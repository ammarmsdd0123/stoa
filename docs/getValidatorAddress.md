###### Endpoint

    https://boascan.io/validator/boa1xrval7gwhjz4k9raqukcnv2n4rl4fxt74m2y9eay6l5mqdf4gntnzhhscrh

HTTP Method: **GET**
<br/>
<br/>
     * Returns a set of Validators based on the block height if there is a height.
     * If height was not provided the latest validator set is returned.
     * If an address was provided, return the validator data of the address if it exists

| Parameter | Explanation  | Example                              |
| --------- | ------------ | ------------------------------------ |
| address   | validator address  | boa1xrval7gwhjz4k9raqukcnv2n4rl4fxt74m2y9eay6l5mqdf4gntnzhhscrh|

Example Response JSON:<br/>
[{"address":"boa1xrval7gwhjz4k9raqukcnv2n4rl4fxt74m2y9eay6l5mqdf4gntnzhhscrh","enrolled_at":"0","stake":"0x210f6551d648a4da654da116b100e941e434e4f232b8579439c2ef64b04819bd2782eb3524c7a29c38c347cdf26006bccac54a58a58f103ae7eb5b252eb53b64","preimage":{"height":"","hash":"0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000"}}]