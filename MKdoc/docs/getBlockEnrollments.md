###### Endpoint

    https://boascan.io//block-enrollments?height=0

HTTP Method: **GET**

@returns enrolled validators of block.

| Query String | Explanation    | Example                            |
| ------------ | -------------- | ---------------------------------- |
| height      | height of block | 0 |

Example Response JSON:<br/>
[{"height":"0","utxo":"0x210f6551d648a4da654da116b100e941e434e4f232b8579439c2ef64b04819bd2782eb3524c7a29c38c347cdf26006bccac54a58a58f103ae7eb5b252eb53b64","enroll_sig":"0x018389f5876ebac77ad4c2269415bf8a5b14e2374e9d30a933f70a10abbca2a40e0122b707d1a0b305efcbca42d73e884987396248c66d329bca486a39735f8c","commitment":"0xcfc5b09bc53136c1691e0991ffae7f2657bba248da07fb153ddf08a5109ce1c7d38206bfab6da57d70c428286d65081db992fbade6c67b97c62e9cb2862433e1","cycle_length":20,"full_count":1}]