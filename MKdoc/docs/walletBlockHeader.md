###### Endpoint

    https://boascan.io//wallet/blocks/header

HTTP Method: **GET**

Returns information about the header of the block according to the height of the block.
If height was not provided the information of the last block header is returned.

| Query String | Explanation    | Example                            |
| ------------ | -------------- | ---------------------------------- |


Example Response JSON:<br/>
{"height":"15","hash":"0x7442e991b1f034febdc068294ac0a7670e4c03dee7dfe1bacc3d6f58258b9a95da65583d2ec211eede645623dedb6eab61bb042b0477d20b3715549d15a14e0a","merkle_root":"0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000","time_stamp":1631852986}