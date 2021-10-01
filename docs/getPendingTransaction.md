###### Endpoint

    https://boascan.io/transaction/pending/0xcb5f52b8954f731003e8c5c3e3e84bb39c7ce8c6a764f8575d55564f7f534b92d3aee51f24a4b57fec52c90910e9fb29509c6e83cbf2299b224cbb3a91bf54d1

HTTP Method: **GET**

Returns a pending transaction by the transaction hash.

| Query String | Explanation      | Example                                      |
| ------------ | ---------------- | -------------------------------------------- |
| hash  | The hash of the transaction to get | 0xcb5f52b8954f731003e8c5c3e3e84bb39c7ce8c6a764f8575d55564f7f534b92d3aee51f24a4b57fec52c90910e9fb29509c6e83cbf2299b224cbb3a91bf54d1 |

Example Request JSON:<br/>
{"inputs":[{"utxo":"0xb9794167a781561298bcb0f634346c85e56fba3f26c641e52dbf0066e8fb0b96d278cdd4c22c7e9885fceb307368e4130aaebd7800905c27c6a6e09870d8d9ca","unlock":{"bytes":"CyJB0TZoWFGZ4OVw1F7zeqX/58jONKaZw/WFmZLT9Q/ZBYxrtWDy59ZuNBSJhdcnnM1Wm/CM/eb86UgAY75yyQE="},"unlock_age":0}],"outputs":[{"type":0,"value":"120000000","lock":{"type":0,"bytes":"jHGh87fbrTK0CUjHDahTRXZuWIANxxOgmGHMn8xbEWM="}},{"type":0,"value":"609999879745200","lock":{"type":0,"bytes":"kZnmFMJObP4+SLxUChUrKaFP/7ek7wIYk79A66URrHE="}}],"payload":"","lock_height":"0"}
